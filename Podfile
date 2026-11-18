
source 'https://mirrors.tuna.tsinghua.edu.cn/git/CocoaPods/Specs.git'
platform :ios, '17.0'

project 'Legado.xcodeproj'

use_frameworks!

target 'Legado' do
  pod 'Alamofire'
  pod 'SwiftSoup', '2.11.3'
  pod 'GCDWebServer', '3.5.4'
  pod 'Kanna', '~> 5.3'
  pod 'SwCrypt', :git => 'https://github.com/jiangjiahuang39-design/SwCrypt.git', :branch => 'master'
end

target 'swiftLegadoTests' do
  pod 'Alamofire'
  pod 'SwiftSoup', '2.11.3'
  pod 'GCDWebServer', '3.5.4'
  pod 'Kanna', '~> 5.3'
  pod 'SwCrypt', :git => 'https://github.com/jiangjiahuang39-design/SwCrypt.git', :branch => 'master'
end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '17.0'
    end
  end
end
