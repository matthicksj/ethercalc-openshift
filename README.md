EtherCalc on OpenShift
======================

This git repository helps you get up and running quickly w/ a EtherCalc installation
on OpenShift. There is no Redis support in opensift for now, so this will fallback on
using disk based json data. I am not sure this will survive a reboot.
 
Running on OpenShift
----------------------------

Create an account at http://openshift.redhat.com/

Create a nodejs application (using the downloadable cartridge) with this code
    rhc create-app ethercalc http://bit.ly/145aBI5
--from-code=https://github.com/matthicksj/ethercalc-openshift
    
That's it, you can now checkout your application at :

    http://ethercalc-$yournamespace.rhcloud.com


