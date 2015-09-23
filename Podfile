workspace 'RunMan.xcworkspace'
xcodeproj 'RunMan.xcodeproj'

inhibit_all_warnings!
platform:ios,'7.0'
#pod install --verbose --no-repo-update

#本地库
pod 'CQTFoundation',  :git => 'https://ANineOK@bitbucket.org/ANineTeam/cqtfoundation.git'
pod 'CQTCoreData',    :git => 'https://ANineOK@bitbucket.org/ANineTeam/cqtcoredata.git'
pod 'CQTLocationKit', :git => 'https://ANineOK@bitbucket.org/ANineTeam/cqtlocationkit.git'
pod 'CQTUIKit',       :git => 'https://ANineOK@bitbucket.org/ANineTeam/cqtuikit.git'
pod 'CQTMediaKit',    :git => 'https://ANineOK@bitbucket.org/ANineTeam/cqtmediakit.git'
pod 'CQTNetworkKit',  :git => 'https://ANineOK@bitbucket.org/ANineTeam/cqtnetworkkit.git'
pod 'CQTJSON',        :git => 'https://ANineOK@bitbucket.org/ANineTeam/cqtjson.git'

#远程库
pod 'ReactiveCocoa', '~> 2.5'
pod 'Masonry', '~> 0.6.2'
pod 'AMap2DMap', '~> 2.6.0'
pod 'AMapSearch', '~> 2.5.0'

post_install do |installer|
    installer.project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['ENABLE_STRICT_OBJC_MSGSEND'] = "NO"
        end
    end
end