# Hello cloud developers,

This is the github.io source code page for [azure.github.io](http://azure.github.io). Please feel free to fork and
submit a pull request if you want to correct or add some content.

Cheers!

## Get Started

- Install Ruby and the Ruby DevKit on your system of choice.

    **Note** If you're running Ruby on a Windows machine, make sure your DevKit path variables are setup using the Dev Kit [quickstart instructions](https://github.com/oneclick/rubyinstaller/wiki/development-kit#quick-start).
- Run `bundle install` from the root of the project. Note: If you do not have Bundler installed, run `gem install bundler` beforehand.
- If you're on Windows, CoffeeScript will cause an error to be thrown when you start building the site. So, do the following steps beforehand:
	- Add the following to your Gemfile:
		```gem 'coffee-script-source', '1.8.0'```
	- Then, run the following:
		```bundle update coffee-script-source```
	- Restart the server, if needed.

## Usage

- To build the site, run `rake build`.

  **Note** Because there's a dependency on ImageMagick, if you're trying to do this on a Windows machine, you'll have to [install ImageMagick](http://www.imagemagick.org/script/binary-releases.php#windows) before the `rake build` operation will succeed.
- If you're running Windows, you need to do the following changes before you can run `rake serve`:
	- ```gem uni hitimes```
	- Remove **ALL** versions of hitimes.
	- Run ```gem ins hitimes -v 1.2.2 --platform ruby```
- To build, start and update the site upon changes, run `rake serve`.
- To publish the site, run `rake publish`.

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request that targets the Jekyll branch. *The master branch is intended for generated html only, not contributions.*

## License and Copyright

*[azure.github.io](http://azure.github.io)* is free software released under the [MIT License](http://www.opensource.org/licenses/MIT).