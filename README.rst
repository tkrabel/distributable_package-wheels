TODO: add status badges here

######################
dispypkg wheel builder
######################

Repository to build wheels.

Edit `appveyor.yml` and `.travis.yml` to change the `BUILD_COMMIT` environment
variable to set the name of the git tag to build, commit and push (to master).

Travis and appveyor should automatically build and test that version on
Windows, Linux and OSX for various versions of Python (both 32 bit and 64 bit).

If the tests pass, the resulting wheels should show up on:

  [Specify the URL]

The following tool can be useful to download all the wheels for a specific
release:

  https://github.com/ogrisel/wheelhouse-uploader

and then use `twine` to publish all the wheels along with the locally built
source tarball of the release all at once to PyPI. 
