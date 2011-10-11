# README
Please note that this is a Darwin-specific fork of the passwdqc-1.2.2 project, available from <http://www.openwall.com/passwdqc/>. Refer to README.dist for the original README file that came with the package.

## Description
passwdqc is a password/passphrase strength checking and policy enforcement toolset, including a PAM module (pam_passwdqc), command-line programs (pwqcheck and pwqgen), and a library (libpasswdqc).

pam_passwdqc is normally invoked on password changes by programs such as passwd(1). It is capable of checking password or passphrase strength, enforcing a policy, and offering randomly-generated passphrases, with all of these features being optional and easily (re-)configurable.

pwqcheck and pwqgen are standalone password/passphrase strength checking and random passphrase generator programs, respectively, which are usable from scripts.

libpasswdqc is the underlying library, which may also be used from third-party programs.

## Installation
All components of passwdqc (the library, the PAM module, and two command-line programs) can be built by simply running "make". To install, run "make install". To uninstall, run "make uninstall".

On the other hand, you may also build everything but the PAM module with "make utils". To install, run "make install_lib install_utils". To uninstall, run "make remove_lib remove_utils".

Please note that this Darwin fork of passwdqc installs into local directories such as /usr/local/etc, /usr/local/lib, /usr/local/lib, /usr/local/include, /usr/local/share/man, /usr/local/bin, /usr/lib/pam.

Please refer to README and PLATFORMS for information on configuring your system to use the PAM module. You may also refer to the pam_passwdqc(8) and passwdqc.conf(5) manual pages.

Please refer to the pwqcheck(1) and pwqgen(1) manual pages for
information on using the command-line programs.

# Credits
http://www.openwall.com/passwdqc/
