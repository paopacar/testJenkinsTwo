# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'testJenkinsTwo' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!
	pod 'AFNetworking'
  # Pods for testJenkinsTwo

  target 'testJenkinsTwoTests' do
    inherit! :search_paths
    # Pods for testing
  end

  target 'testJenkinsTwoUITests' do
    inherit! :search_paths
    # Pods for testing
  end

end

post_install do |installer|
  installer.pods_project.build_configuration_list.build_configurations.each do |configuration|
    configuration.build_settings['CLANG_ALLOW_NON_MODULAR_INCLUDES_IN_FRAMEWORK_MODULES'] = 'YES'
  end
end
