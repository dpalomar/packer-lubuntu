# Packer Ubuntu 16.04 minimal Desktop Vagrant Box

**Current Ubuntu Version Used**: 16.04.1

This projects generates a minimal desktop image based on Lubuntu core.
Clean desktop whitout heavy software installed.



  - VirtualBox
  - VMware
  

## Requirements

- Packer



## Usage

Make sure all the required software (listed above) is installed, then cd to the directory containing this README.md file, and run:

    $ packer build ubuntu1604.json

After a few minutes, Packer should tell you the box was generated successfully.

You could use `vagrant init dpalomar/Lubuntu1604; vagrant up` instead if you simply prefer the built image. (_WARNING:_ you must change the Vagranfile before `vagrant up` to show the gui)

If you want to only build a box for one of the supported virtualization platforms (e.g. only build the VMware box), add `--only=vmware-iso` to the `packer build` command:

    $ packer build --only=vmware-iso ubuntu1604.json

## License

MIT license.

## Author Information

Created in 2016 by David Palomar, template based on Jeff Geerling and Bento project. 
