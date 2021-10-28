# nodejsporter

#### Description
nodejsporter is a rpm packager bot for nodejs modules from npmjs.org.
It is a tool used to create spec and rpm files for nodejs modules.


#### Installation Command

  python3 setup.py install

#### Preparation
Install the following software (YUM) before using this tool:
1.  gcc
2.  gdb
3.  libstdc++-devel
4.  python3-cffi
5.  nodejs

 **rpm -ivh nodejs-packaging-23-1.noarch.rpm**  at the URL:
https://gitee.com/chendong1995/nodejs-packaging?_from=gitee_search

#### Instructions

nodejsporter is a tool used to create spec and rpm files for nodejs modules.
For more details, run  **nodejsporter –h**.

`nodejsporter <package> -s -b -d -o  nodejs-<package>.spec`

#### Contribution

1.  Fork the repository.
2.  Create the Feat_xxx branch.
3.  Commit your code.
4.  Create a Pull Request (PR).

#### How to Create a rpm File

1.  Create a spec file:  **nodejsporter -s module_name** 
2.  Obtain required nodejsmodules:  **nodejsporter -R module_name** 
3.  Build and install rpm package:  **nodejsporter -B module_name** 
4.  Specify a version:  **nodejsporter -B module_name 1.0.0** 
5.  Obtain more detail:  **nodejsporter –h** 
