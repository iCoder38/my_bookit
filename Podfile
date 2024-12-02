# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'Bookit' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!

  # Pods for Bookit

  pod 'FSCalendar'

  # webservice
  pod 'Alamofire'
  pod 'SwiftyJSON'
  pod 'SDWebImage'
  pod 'GrowingTextView'
  pod 'SwiftGifOrigin'
  pod 'SPConfetti'
  pod 'BSImagePicker', '~> 3.1'
  pod 'OpalImagePicker'
  pod 'QCropper'
  pod 'Firebase'
  pod 'Firebase/Auth'
  pod 'Firebase/Database'
  # pod 'ChameleonFramework'
  pod 'Firebase/Analytics'
  pod 'Firebase/Messaging'
  pod 'Firebase/Analytics'
  # pod 'Stripe', '19.0.1'
  pod 'SquareInAppPaymentsSDK'

  target 'BookitTests' do
    inherit! :search_paths
    # Pods for testing
  end

  target 'BookitUITests' do
    # Pods for testing
  end

end

# Post-install script to avoid duplicate embedding of frameworks
post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['EXPANDED_CODE_SIGN_IDENTITY'] = nil
      config.build_settings['CODE_SIGNING_REQUIRED'] = "NO"
    end
  end
end

