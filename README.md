# saltpatches
Bitfusion.io patches for Saltstack

## patches

Quilt stack containing:
- docker_device - add a passthrough for the Docker "devices" keyword

  To install this patch you need the "quilt" utility
  
  This patch applies to version 2015.8.1 of Saltstack and should be installed on the *minion* as well as the master
  
  You should use the latest version of docker-py.
  
      # pip install --upgrade docker-py
  
  If you get a client/server mismatch error, force the protocol version using
  
      # salt 'myminion' grains.setval '"1.19"'
      
  Note the quoting to ensure this is a string value type not a float
  


