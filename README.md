1. Download Python 2 from the Arch Arm repositories (armv7h)
    <!-- * http://mirror.archlinuxarm.org/armv7h/extra/python2-2.7.18-5.1-armv7h.pkg.tar.xz -->
    * https://archlinuxarm.org/packages/armv7h/python

2. Extract to \<repo-root>/bootstrap-python/python3
  * Should be:
    \<repo-root>/bootstrap-python/python3/usr/...

3. Ensure you can ssh to your reMarkable

4. Add a `Host` entry to your .ssh/config named `remarkable` with `User root` directive

4. Edit host_vars/remarkable.yaml to include your templates

5. Run `ansible-playbook -i inventory.yaml playbook.yaml`