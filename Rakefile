# -*- coding: utf-8 -*-
$:.unshift("/Library/RubyMotion/lib")
require 'motion/project/template/ios'

begin
  require 'bundler'
  Bundler.require
rescue LoadError
end

Dotenv.load

Motion::Project::App.setup do |app|
  # Use `rake config' to see complete project settings.
  app.name = 'pixate_test'

  app.pods do
    pod 'Pixate'
  end
  app.pixate.user = ENV['PIXATE_USER']
  app.pixate.key  = ENV['PIXATE_KEY']
  app.pixate.framework = 'vendor/Pods/Pixate/Framework/iOS/Pixate.framework/'
end
