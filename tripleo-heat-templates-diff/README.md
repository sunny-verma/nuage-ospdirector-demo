Steps:

Clone this repo onto the undercloud machine   

```
git clone https://gitlab.us.alcatel-lucent.com/sunnyve/OSPDInstallDocumentation.git
cd OSPDInstallDocumentation
cd tripleo-heat-templates-diff/
```

<b>For Non AVRS integration,</b>

Run either `sudo ./apply_patch.py` or `sudo python apply_patch.py` to patch the changes.   

<b>For AVRS integration,</b>

Run either `sudo ./apply_patch.py avrs` or  `sudo python apply_patch.py avrs` to patch the changes.


Verify that all the changes are applied. Ensure that there are no "Hunk #1 FAILED" errors. There might be "hunk ignored" warnings (based on running version) which can be ignored.   

Multiple versions are supported by the script: openstack-tripleo-heat-templates-8.0.2-4.el7ost.noarch, openstack-tripleo-heat-templates-8.0.2-43.el7ost.noarch, openstack-tripleo-heat-templates-8.0.4-20.el7ost.noarch and openstack-tripleo-heat-templates-8.0.7-4.el7ost.noarch

