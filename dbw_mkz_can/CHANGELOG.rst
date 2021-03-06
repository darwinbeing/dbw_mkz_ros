^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package dbw_mkz_can
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

1.0.6 (2017-06-21)
------------------
* Added frame_id parameter for IMU and Twist messages
* Properly handle IMU unknown covariance and fields that are not present
* Removed SuspensionReport (data was unintelligible)
* Reorganized launch files.
* Swapped lateral and longitudinal acceleration in IMU message.
* Export dispatch.h for use by other packages
* Added clear bit to command messages
* Updated nodelet to the PLUGINLIB_EXPORT_CLASS macro
* Additional dependencies
* Contributors: Kevin Hallenbeck, Micho Radovnikovich

1.0.5 (2017-04-25)
------------------
* Updated package.xml format to version 2
* Unique target names
* Contributors: Kevin Hallenbeck

1.0.4 (2016-12-06)
------------------
* Added brake and throttle thrashing scripts to try and induce faults
* Changed wheel speeds to signed values
* Contributors: Kevin Hallenbeck, Joshua Whitley

1.0.3 (2016-11-17)
------------------
* Added QUIET bit to disable driver override audible warning
* Print brake/throttle/steering firmware versions
* Handle and report steering faults (FLTBUS1 and FLTBUS2)
* Contributors: Kevin Hallenbeck

1.0.2 (2016-11-07)
------------------
* Configurable steering ratio
* Contributors: Kevin Hallenbeck

1.0.1 (2016-10-10)
------------------
* Added support for apt-get binary packages
* Added twist message computed from vehicle speed and steering wheel angle.
* Contributors: Kevin Hallenbeck

1.0.0 (2016-09-28)
------------------
* Initial release
* Contributors: Kevin Hallenbeck, Micho Radovnikovich
