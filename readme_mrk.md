This is mark's installation of RescueOMR from:
https://github.com/EuracBiomedicalResearch/RescueOMR
I'm tweaking the installation to use a venv for dependency isolation.

Since the project needs python3 the venv is setup using
py3's native approach:
python3 -m venv ./venv
activate with source ./bin/activate # often alisased to 'activate' in bash_profile

also remember to use pip3 instead of pip

Note that the bin/ dir contains two files that are actually
python scripts.  The bin/ dir-name from RescueOMR :(

Dependencies
* PIL is an old, dead project so installed Pillow instead.  But seems
that one still imports from PIL.
* numpy seems to have brought scipy with it so that was installed
separately
* skimage seems to want to be installs as scikit-image

NEXT
* install dependencies for RescueOMR
