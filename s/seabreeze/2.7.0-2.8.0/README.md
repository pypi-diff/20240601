# Comparing `tmp/seabreeze-2.7.0.tar.gz` & `tmp/seabreeze-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seabreeze-2.7.0.tar", last modified: Wed Feb 21 22:40:39 2024, max compression
+gzip compressed data, was "seabreeze-2.8.0.tar", last modified: Sat Jun  1 06:55:38 2024, max compression
```

## Comparing `seabreeze-2.7.0.tar` & `seabreeze-2.8.0.tar`

### file list

```diff
@@ -1,1200 +1,1200 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.998012 seabreeze-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-21 22:40:23.000000 seabreeze-2.7.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-02-21 22:40:23.000000 seabreeze-2.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-02-21 22:40:23.000000 seabreeze-2.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-02-21 22:40:23.000000 seabreeze-2.7.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-21 22:40:23.000000 seabreeze-2.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-02-21 22:40:38.998012 seabreeze-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-02-21 22:40:23.000000 seabreeze-2.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.814013 seabreeze-2.7.0/dev/
--rw-r--r--   0 runner    (1001) docker     (127)    10264 2024-02-21 22:40:23.000000 seabreeze-2.7.0/dev/pretty_print_obp_pcapng.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.814013 seabreeze-2.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-21 22:40:23.000000 seabreeze-2.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-21 22:40:23.000000 seabreeze-2.7.0/docs/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.818013 seabreeze-2.7.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.818013 seabreeze-2.7.0/docs/source/_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-02-21 22:40:23.000000 seabreeze-2.7.0/docs/source/_extensions/repo_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.818013 seabreeze-2.7.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    36848 2024-02-21 22:40:23.000000 seabreeze-2.7.0/docs/source/_static/overview.png
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-02-21 22:40:23.000000 seabreeze-2.7.0/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-02-21 22:40:23.000000 seabreeze-2.7.0/docs/source/backend_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-02-21 22:40:23.000000 seabreeze-2.7.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-02-21 22:40:23.000000 seabreeze-2.7.0/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-02-21 22:40:23.000000 seabreeze-2.7.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-02-21 22:40:23.000000 seabreeze-2.7.0/docs/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-02-21 22:40:23.000000 seabreeze-2.7.0/docs/source/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-02-21 22:40:23.000000 seabreeze-2.7.0/docs/source/tldr.rst
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-02-21 22:40:23.000000 seabreeze-2.7.0/docs/source/troubleshoot.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.818013 seabreeze-2.7.0/os_support/
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-02-21 22:40:23.000000 seabreeze-2.7.0/os_support/10-oceanoptics.rules
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-02-21 22:40:23.000000 seabreeze-2.7.0/os_support/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)  7255559 2024-02-21 22:40:23.000000 seabreeze-2.7.0/os_support/windows-driver-files.zip
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-02-21 22:40:23.000000 seabreeze-2.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-21 22:40:23.000000 seabreeze-2.7.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-21 22:40:23.000000 seabreeze-2.7.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 22:40:38.998012 seabreeze-2.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-02-21 22:40:23.000000 seabreeze-2.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.810013 seabreeze-2.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.802013 seabreeze-2.7.0/src/libseabreeze/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.794013 seabreeze-2.7.0/src/libseabreeze/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.826013 seabreeze-2.7.0/src/libseabreeze/include/api/
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/DeviceFactory.h
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/USBEndpointTypes.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.834013 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/AcquisitionDelayFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/ContinuousStrobeFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/DHCPServerFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/DataBufferFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)    28448 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/DeviceAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/EEPROMFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/EthernetConfigurationFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/FastBufferFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/FeatureAdapterInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/FeatureAdapterTemplate.h
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/FeatureFamilies.h
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/I2CMasterFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/IPv4FeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/IntrospectionFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/IrradCalFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/LightSourceFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/MulticastFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/NetworkConfigurationFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/NonlinearityCoeffsFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/OpticalBenchFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/PixelBinningFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/ProtocolFamilies.h
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/RawUSBBusAccessFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/RevisionFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)    29520 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPI.h
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPIConstants.h
--rw-r--r--   0 runner    (1001) docker     (127)    26268 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPI_Impl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/SerialNumberFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/ShutterFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/SpectrometerFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/SpectrumProcessingFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/StrayLightCoeffsFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/StrobeLampFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/TemperatureFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/ThermoElectricCoolerFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/WifiConfigurationFeatureAdapter.h
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/gpioFeatureAdapter.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.838013 seabreeze-2.7.0/src/libseabreeze/include/common/
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/ByteVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/Data.h
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/DoubleVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/FloatVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/Log.h
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/SeaBreeze.h
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/U32Vector.h
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/UShortVector.h
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/UnitDescriptor.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.838013 seabreeze-2.7.0/src/libseabreeze/include/common/buses/
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/buses/Bus.h
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/buses/BusFamilies.h
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/buses/BusFamily.h
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/buses/DeviceLocationProberInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/buses/DeviceLocatorInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/buses/TransferHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.838013 seabreeze-2.7.0/src/libseabreeze/include/common/buses/network/
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/buses/network/IPv4NetworkProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/buses/network/IPv4SocketDeviceLocator.h
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/buses/network/TCPIPv4SocketBus.h
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/buses/network/TCPIPv4SocketTransferHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.838013 seabreeze-2.7.0/src/libseabreeze/include/common/buses/rs232/
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/buses/rs232/RS232DeviceLocator.h
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/buses/rs232/RS232Interface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/buses/rs232/RS232TransferHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.838013 seabreeze-2.7.0/src/libseabreeze/include/common/buses/usb/
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/buses/usb/USBDeviceLocator.h
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/buses/usb/USBInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/buses/usb/USBTransferHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.838013 seabreeze-2.7.0/src/libseabreeze/include/common/devices/
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/devices/Device.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.842013 seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/BusConnectException.h
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/BusException.h
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/BusTransferException.h
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/FeatureControlException.h
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/FeatureException.h
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/FeatureProtocolNotFoundException.h
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/IllegalArgumentException.h
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/NumberFormatException.h
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/ProtocolBusMismatchException.h
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/ProtocolException.h
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/ProtocolFormatException.h
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/ProtocolTransactionException.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.842013 seabreeze-2.7.0/src/libseabreeze/include/common/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/features/Feature.h
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/features/FeatureFamily.h
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/features/FeatureImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/globals.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.842013 seabreeze-2.7.0/src/libseabreeze/include/common/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/protocols/Exchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/protocols/Protocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/protocols/ProtocolFamily.h
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/protocols/ProtocolHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/protocols/ProtocolHint.h
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/protocols/Transaction.h
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/common/protocols/Transfer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.794013 seabreeze-2.7.0/src/libseabreeze/include/native/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.846013 seabreeze-2.7.0/src/libseabreeze/include/native/network/
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/native/network/Inet4Address.h
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/native/network/Socket.h
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/native/network/SocketException.h
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/native/network/SocketTimeoutException.h
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/native/network/UnknownHostException.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.846013 seabreeze-2.7.0/src/libseabreeze/include/native/network/posix/
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/native/network/posix/NativeSocketPOSIX.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.846013 seabreeze-2.7.0/src/libseabreeze/include/native/network/windows/
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/native/network/windows/NativeSocketWindows.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.846013 seabreeze-2.7.0/src/libseabreeze/include/native/rs232/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/native/rs232/NativeRS232.h
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/native/rs232/RS232.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.846013 seabreeze-2.7.0/src/libseabreeze/include/native/rs232/windows/
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/native/rs232/windows/NativeRS232Windows.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.846013 seabreeze-2.7.0/src/libseabreeze/include/native/system/
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/native/system/NativeSystem.h
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/native/system/System.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.846013 seabreeze-2.7.0/src/libseabreeze/include/native/usb/
--rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/native/usb/NativeUSB.h
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/native/usb/USB.h
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/native/usb/USBDiscovery.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.846013 seabreeze-2.7.0/src/libseabreeze/include/native/usb/winusb/
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/native/usb/winusb/WindowsGUID.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.794013 seabreeze-2.7.0/src/libseabreeze/include/vendors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.802013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.794013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.846013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/network/
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/network/FlameXTCPIPv4.h
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/network/JazTCPIPv4.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.846013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/rs232/
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/rs232/OOIRS232Interface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.854013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/ApexUSB.h
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameNIRUSB.h
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameXUSB.h
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameXUSBTransferHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR2000PlusUSB.h
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR2000USB.h
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR4000USB.h
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/JazUSB.h
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/Maya2000ProUSB.h
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/Maya2000USB.h
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/MayaLSLUSB.h
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/NIRQuest256USB.h
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/NIRQuest512USB.h
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSB4KSpectrumTransferHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBControlTransferHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBEndpointMaps.h
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBProductID.h
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBSpectrumTransferHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBTrivialTransferHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/QE65000USB.h
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/QEProUSB.h
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/STSUSB.h
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/SparkUSB.h
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/TorusUSB.h
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB2000PlusUSB.h
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB2000USB.h
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB4000USB.h
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/VentanaUSB.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.858013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/Apex.h
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/FlameNIR.h
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/FlameX.h
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR2000.h
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR2000Plus.h
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR4000.h
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/Jaz.h
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/Maya2000.h
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/Maya2000Pro.h
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/MayaLSL.h
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/NIRQuest256.h
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/NIRQuest512.h
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/QE65000.h
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/QEPro.h
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/STS.h
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/Spark.h
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/Torus.h
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB2000.h
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB2000Plus.h
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB4000.h
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/Ventana.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.798013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.858013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature_FPGA.h
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/STSAcquisitionDelayFeature.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.858013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature_FPGA.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.858013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/DataBufferFeatureBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/DataBufferFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/FlameXDataBufferFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/QEProDataBufferFeature.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.858013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/dhcp_server/
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/dhcp_server/DHCPServerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/dhcp_server/DHCPServerFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.862013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/NonlinearityEEPROMSlotFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeatureBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_MayaPro.h
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_NIRQuest.h
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SerialNumberEEPROMSlotFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/StrayLightEEPROMSlotFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature_QE65000.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.862013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/ethernet_configuration/
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.862013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FlameXFastBufferFeature.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.862013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/fpga_register/
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/fpga_register/FPGARegisterFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/fpga_register/FPGARegisterFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.862013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/gpio/
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/gpio/gpioFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/gpio/gpioFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.862013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/i2c_master/
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/i2c_master/i2cMasterFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/i2c_master/i2cMasterFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.862013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/introspection/
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/introspection/IntrospectionFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/introspection/IntrospectionFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.862013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/ipv4/
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/ipv4/IPv4Feature.h
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/ipv4/IPv4FeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.866013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/irradcal/
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/irradcal/IrradCalFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/irradcal/IrradCalFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.866013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/StrobeLampFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/StrobeLampFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/VentanaLightSourceFeature.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.866013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/multicast/
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/multicast/MulticastFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/multicast/MulticastFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.866013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/network_configuration/
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.866013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/nonlinearity/
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.866013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/optical_bench/
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/optical_bench/OpticalBenchFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/optical_bench/OpticalBenchFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.866013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/pixel_binning/
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/pixel_binning/PixelBinningFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/pixel_binning/STSPixelBinningFeature.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.866013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/raw_bus_access/
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.866013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/revision/
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/revision/RevisionFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/revision/RevisionFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.870013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/serial_number/
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/serial_number/SerialNumberFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/serial_number/SerialNumberFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.870013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/shutter/
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/shutter/ShutterFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/shutter/ShutterFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.874013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ApexSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/FlameNIRSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/FlameXSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/GainAdjustedSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR2000PlusSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR2000SpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR4000SpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/JazSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/Maya2000ProSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/Maya2000SpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/MayaLSLSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuest256SpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuest512SpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuestSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureImpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/QE65000SpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/QEProSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/STSSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/SparkSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/SpectrometerTriggerMode.h
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB2000PlusSpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB2000SpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB4000SpectrometerFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/VentanaSpectrometerFeature.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.874013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrum_processing/
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.874013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/stray_light/
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.874013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/temperature/
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/temperature/TemperatureFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/temperature/TemperatureFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.874013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/QEProThermoElectricFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureBase.h
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricQEFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/VentanaThermoElectricFeature.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.874013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/wavecal/
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/wavecal/WaveCalFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/wavecal/WaveCalFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.874013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/wifi_configuration/
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeature.h
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeatureInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.802013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.882013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/AcquisitionDelayProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ContinuousStrobeProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/DHCPServerProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/DataBufferProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/EEPROMProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/EthernetConfigurationProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/FPGARegisterProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/FastBufferProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/GPIOProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/I2CMasterProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IPv4ProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IntrospectionProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IrradCalProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/LightSourceProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/MulticastProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/NetworkConfigurationProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/NonlinearityCoeffsProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/OpticalBenchProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/PixelBinningProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ProgrammableSaturationProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/RevisionProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SerialNumberProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ShutterProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SpectrometerProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SpectrumProcessingProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/StrayLightCoeffsProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/StrobeLampProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/TemperatureProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ThermoElectricProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/WaveCalProtocolInterface.h
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/WifiConfigurationProtocolInterface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.802013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.882013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/constants/
--rw-r--r--   0 runner    (1001) docker     (127)    21778 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/constants/OBPMessageTypes.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.902013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPAddIPv4AddressExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPCommand.h
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobeEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobePeriodExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferClearExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferRemoveOldestExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDeleteIPv4AddressExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetActivePixelRangesExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetAllTemperaturesExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetBoxcarWidthExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetConsecutiveSampleCountExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerAddressExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCapacityExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferElementCountExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferMaximumCapacityExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDefaultPixelBinningExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetElectricDarkPixelRangesExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationGbEEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationMACAddressExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFastBufferingEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFirmwareRevisionExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionAvailableModesExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionCurrentModeExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionNumberOfPinsExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionOutputVectorExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionValueExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIONumberOfPinsExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOOutputEnableVectorExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOValueVectorExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetHardwareRevisionExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetI2CMasterNumberOfBusesExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4AddressExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DHCPEnableStateExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DefaultGatewayExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4NumberOfAddressesExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCalExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCollectionAreaExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMaxPixelBinningExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMulticastEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceConnectionTypeExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceEnableStateExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffsCountExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfNetworkInterfacesExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfPixelsExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchCoatingExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFiberDiameterMicronsExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFilterExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchGratingExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchIDExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSerialNumberExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSlitWidthMicronsExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalDarkPixelRangesExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetPixelBinningExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSaturationExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetScansToAverageExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberMaximumLengthExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffsCountExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureCountExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetThermoElectricTemperatureExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWaveCalExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationModeExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSSIDExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSecurityExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPIntegrationTimeExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLampEnableCommand.h
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnableCommand.h
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnabledQuery.h
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityCommand.h
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityQuery.h
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPMessage.h
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPQuery.h
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadI2CMasterBusExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadNumberOfRawSpectraWithMetadataExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrum32AndMetadataExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrum32AndMetadataExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumWithGainExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestBufferedSpectrum32AndMetadataExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestNumberOfBufferedSpectraWithMetadataExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestRawSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRunNetworkInterfaceSelfTestExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSaveNetworkInterfaceConnectionSettingsExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetAcquisitionDelayExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetBoxcarWidthExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetConsecutiveSampleCountExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerAddressExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDataBufferCapacityExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDefaultPixelBinningExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationGbEEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationMACAddressExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetFastBufferingEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionModeExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionOutputVectorExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionValueExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionVectorExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOOutputEnableVectorExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOValueVectorExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DHCPEnableStateExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DefaultGatewayExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCalExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCollectionAreaExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetMulticastEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetNetworkInterfaceEnableStateExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetPixelBinningExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetScansToAverageExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricSetpointExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationModeExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationPassPhraseExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSSIDExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSecurityExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPShutterExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPTransaction.h
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPTriggerModeExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPWriteI2CMasterBusExchange.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.902013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/hints/
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/hints/OBPControlHint.h
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/hints/OBPSpectrumHint.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.906013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPAcquisitionDelayProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPContinuousStrobeProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPDHCPServerProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPDataBufferProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPEthernetConfigurationProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPFastBufferProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPGPIOProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPI2CMasterProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIPv4Protocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIntrospectionProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIrradCalProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol_Ventana.h
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPMulticastProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPNetworkConfigurationProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPNonlinearityCoeffsProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPOpticalBenchProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPPixelBinningProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPProgrammableSaturationProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPRevisionProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSerialNumberProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPShutterProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSpectrometerProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSpectrumProcessingProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPStrayLightCoeffsProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPStrobeLampProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPTemperatureProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPThermoElectricProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPWaveCalProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPWifiConfigurationProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OceanBinaryProtocol.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.802013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.906013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/FPGARegisterCodes.h
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/OpCodes.h
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/QETECConstants.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.910013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterReadExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterWriteExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGASpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FlameNIRSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/HRFPGASpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/IntegrationTimeExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/JazSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/MayaProSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/NIRQuestSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOI2KSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIIrradCalExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIReadIrradCalExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIWriteIrradCalExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/QESpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadEEPROMSlotExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECQETemperatureExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECTemperatureExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/RequestSpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/StrobeEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TECEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TECQEEnableExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TriggerModeExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/USBFPGASpectrumExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteEEPROMSlotExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECQESetPointExchange.h
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECSetPointExchange.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.910013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/hints/
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/hints/ControlHint.h
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/hints/SpectrumHint.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.914013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/FPGARegisterProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIEEPROMProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIIrradCalProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOISpectrometerProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIStrobeLampProtocol.h
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOITECProtocol.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.914013 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/utils/Polynomial.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.806013 seabreeze-2.7.0/src/libseabreeze/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.914013 seabreeze-2.7.0/src/libseabreeze/src/api/
--rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/DeviceFactory.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.918012 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/AcquisitionDelayFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/ContinuousStrobeFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/DHCPServerFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/DataBufferFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    80076 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/DeviceAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/EEPROMFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/EthernetConfigurationFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/FastBufferFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12485 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/FeatureFamilies.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/I2CMasterFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/IPv4FeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5019 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/IntrospectionFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/IrradCalFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/LightSourceFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/MulticastFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/NetworkConfigurationFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/NonlinearityCoeffsFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/OpticalBenchFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/PixelBinningFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/ProtocolFamilies.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/RawUSBBusAccessFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/RevisionFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/SeaBreezeAPI.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    87831 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/SeaBreezeAPI_Impl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/SerialNumberFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/ShutterFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/SpectrometerFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/SpectrumProcessingFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/StrayLightCoeffsFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/StrobeLampFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/TemperatureFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/ThermoElectricCoolerFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/WifiConfigurationFeatureAdapter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/gpioFeatureAdapter.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.918012 seabreeze-2.7.0/src/libseabreeze/src/common/
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/ByteVector.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/Data.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/DoubleVector.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/FloatVector.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/Log.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/U32Vector.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/UShortVector.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/UnitDescriptor.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.922013 seabreeze-2.7.0/src/libseabreeze/src/common/buses/
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/buses/Bus.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/buses/BusFamilies.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/buses/BusFamily.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/buses/DeviceLocationProberInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/buses/TransferHelper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.922013 seabreeze-2.7.0/src/libseabreeze/src/common/buses/network/
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/buses/network/IPv4NetworkProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/buses/network/IPv4SocketDeviceLocator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/buses/network/TCPIPv4SocketBus.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/buses/network/TCPIPv4SocketTransferHelper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.922013 seabreeze-2.7.0/src/libseabreeze/src/common/buses/rs232/
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/buses/rs232/RS232DeviceLocator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/buses/rs232/RS232Interface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/buses/rs232/RS232TransferHelper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.922013 seabreeze-2.7.0/src/libseabreeze/src/common/buses/usb/
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/buses/usb/USBDeviceLocator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/buses/usb/USBInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/buses/usb/USBTransferHelper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.922013 seabreeze-2.7.0/src/libseabreeze/src/common/devices/
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/devices/Device.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.922013 seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/BusConnectException.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/BusException.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/BusTransferException.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/FeatureControlException.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/FeatureException.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/FeatureProtocolNotFoundException.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/IllegalArgumentException.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/NumberFormatException.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/ProtocolBusMismatchException.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/ProtocolException.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/ProtocolFormatException.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/ProtocolTransactionException.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.926013 seabreeze-2.7.0/src/libseabreeze/src/common/features/
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/features/FeatureFamily.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/features/FeatureImpl.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.926013 seabreeze-2.7.0/src/libseabreeze/src/common/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/protocols/Exchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/protocols/Protocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/protocols/ProtocolFamily.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/protocols/ProtocolHelper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/protocols/ProtocolHint.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/protocols/Transaction.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/common/protocols/Transfer.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.806013 seabreeze-2.7.0/src/libseabreeze/src/native/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.926013 seabreeze-2.7.0/src/libseabreeze/src/native/network/
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/native/network/Inet4Address.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/native/network/SocketException.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/native/network/SocketTimeoutException.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/native/network/UnknownHostException.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.926013 seabreeze-2.7.0/src/libseabreeze/src/native/network/posix/
--rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/native/network/posix/NativeSocketPOSIX.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.926013 seabreeze-2.7.0/src/libseabreeze/src/native/network/windows/
--rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/native/network/windows/NativeSocketWindows.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.926013 seabreeze-2.7.0/src/libseabreeze/src/native/rs232/
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/native/rs232/RS232.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.926013 seabreeze-2.7.0/src/libseabreeze/src/native/rs232/posix/
--rw-r--r--   0 runner    (1001) docker     (127)    12360 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/native/rs232/posix/NativeRS232POSIX.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.926013 seabreeze-2.7.0/src/libseabreeze/src/native/rs232/windows/
--rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/native/rs232/windows/NativeRS232Windows.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.926013 seabreeze-2.7.0/src/libseabreeze/src/native/system/
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/native/system/System.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.926013 seabreeze-2.7.0/src/libseabreeze/src/native/system/posix/
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/native/system/posix/NativeSystemPOSIX.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.926013 seabreeze-2.7.0/src/libseabreeze/src/native/system/windows/
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/native/system/windows/NativeSystemWindows.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.926013 seabreeze-2.7.0/src/libseabreeze/src/native/usb/
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/native/usb/USB.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/native/usb/USBDiscovery.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.926013 seabreeze-2.7.0/src/libseabreeze/src/native/usb/linux/
--rw-r--r--   0 runner    (1001) docker     (127)    22561 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/native/usb/linux/NativeUSBLinux.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.926013 seabreeze-2.7.0/src/libseabreeze/src/native/usb/osx/
--rw-r--r--   0 runner    (1001) docker     (127)    38021 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/native/usb/osx/NativeUSBMacOSX.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.930013 seabreeze-2.7.0/src/libseabreeze/src/native/usb/winusb/
--rw-r--r--   0 runner    (1001) docker     (127)    28911 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/native/usb/winusb/NativeUSBWinUSB.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.806013 seabreeze-2.7.0/src/libseabreeze/src/vendors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.810013 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.806013 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.930013 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/network/
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/network/FlameXTCPIPv4.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/network/JazTCPIPv4.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.930013 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/rs232/
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/rs232/OOIRS232Interface.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.934013 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/ApexUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameNIRUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameXUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameXUSBTransferHelper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR2000PlusUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR2000USB.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR4000USB.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/JazUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/Maya2000ProUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/Maya2000USB.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/MayaLSLUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/NIRQuest256USB.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/NIRQuest512USB.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSB4KSpectrumTransferHelper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBControlTransferHelper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBEndpointMaps.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBSpectrumTransferHelper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBTrivialTransferHelper.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/QE65000USB.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/QEProUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/STSUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/SparkUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/TorusUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB2000PlusUSB.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB2000USB.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB4000USB.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/VentanaUSB.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.938012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/Apex.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/FlameNIR.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/FlameX.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR2000.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR2000Plus.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR4000.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/Jaz.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/Maya2000.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/Maya2000Pro.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/MayaLSL.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/NIRQuest256.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/NIRQuest512.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/QE65000.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/QEPro.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/STS.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/Spark.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/Torus.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB2000.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB2000Plus.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB4000.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7724 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/Ventana.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.810013 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.938012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature_FPGA.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/STSAcquisitionDelayFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.938012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/continuous_strobe/
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature_FPGA.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.938012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/
--rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/DataBufferFeatureBase.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/FlameXDataBufferFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/QEProDataBufferFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.938012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/dhcp_server/
--rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/dhcp_server/DHCPServerFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.938012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureBase.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/NonlinearityEEPROMSlotFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeatureBase.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_MayaPro.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_NIRQuest.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SerialNumberEEPROMSlotFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/StrayLightEEPROMSlotFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature_QE65000.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.938012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/ethernet_configuration/
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.942012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/fast_buffer/
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureBase.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/fast_buffer/FlameXFastBufferFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.942012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/fpga_register/
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/fpga_register/FPGARegisterFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.942012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/gpio/
--rw-r--r--   0 runner    (1001) docker     (127)    13793 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/gpio/gpioFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.942012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/i2c_master/
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/i2c_master/i2cFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.942012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/introspection/
--rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/introspection/IntrospectionFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.942012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/ipv4/
--rw-r--r--   0 runner    (1001) docker     (127)     9822 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/ipv4/IPv4Feature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.942012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/irradcal/
--rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/irradcal/IrradCalFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.942012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/
--rw-r--r--   0 runner    (1001) docker     (127)    14844 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/LightSourceFeatureBase.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/LightSourceFeatureImpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/StrobeLampFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/VentanaLightSourceFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.942012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/multicast/
--rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/multicast/MulticastFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.942012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/network_configuration/
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.942012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/nonlinearity/
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.942012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/optical_bench/
--rw-r--r--   0 runner    (1001) docker     (127)     9817 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/optical_bench/OpticalBenchFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.942012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/pixel_binning/
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/pixel_binning/PixelBinningFeatureInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/pixel_binning/STSPixelBinningFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.942012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/raw_bus_access/
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.942012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/revision/
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/revision/RevisionFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.942012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/serial_number/
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/serial_number/SerialNumberFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.942012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/shutter/
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/shutter/ShutterFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.946013 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/
--rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ApexSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/FlameNIRSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/FlameXSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/GainAdjustedSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR2000PlusSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR2000SpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR4000SpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/JazSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/Maya2000ProSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/Maya2000SpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/MayaLSLSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuest256SpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuest512SpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuestSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    14571 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureBase.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureImpl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/QE65000SpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/QEProSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/STSSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/SparkSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/SpectrometerTriggerMode.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB2000PlusSpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB2000SpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB4000SpectrometerFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/VentanaSpectrometerFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.946013 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrum_processing/
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.950013 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/stray_light/
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.950013 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/temperature/
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/temperature/TemperatureFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.950013 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/QEProThermoElectricFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureBase.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/ThermoElectricQEFeature.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/VentanaThermoElectricFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.950013 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/wavecal/
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/wavecal/WaveCalFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.950013 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/wifi_configuration/
--rw-r--r--   0 runner    (1001) docker     (127)     9640 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeature.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.810013 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.954012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/AcquisitionDelayProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ContinuousStrobeProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/DHCPServerProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/DataBufferProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/EEPROMProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/EthernetConfigurationProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/FPGARegisterProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/FastBufferProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/GPIOProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/I2CMasterProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IPv4ProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IntrospectionProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IrradCalProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/LightSourceProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/MulticastProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/NetworkConfigurationProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/NonlinearityCoeffsProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/OpticalBenchProtocolInteface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/PixelBinningProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ProgrammableSaturationProtocolInteface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/RevisionProtocolInteface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SerialNumberProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ShutterProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SpectrometerProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SpectrumProcessingProtocolInteface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/StrayLightCoeffsProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/StrobeLampProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/TemperatureProtocolInteface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ThermoElectricProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/WaveCalProtocolInterface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/WifiConfigurationProtocolInterface.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.810013 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.974012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPAddIPv4AddressExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPCommand.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobeEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobePeriodExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferClearExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferRemoveOldestExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDeleteIPv4AddressExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetActivePixelRangesExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetAllTemperaturesExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetBoxcarWidthExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetConsecutiveSampleCountExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerAddressExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCapacityExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCountExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferMaximumCapacityExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDefaultPixelBinningExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetElectricDarkPixelRangesExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationGbEEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationMACAddressExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFastBufferingEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFirmwareRevisionExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionAvailableModesExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionCurrentModeExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionNumberOfPinsExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionOutputVectorExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionValueExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIONumberOfPinsExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOOutputEnableVectorExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOValueVectorExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetHardwareRevisionExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetI2CMasterNumberOfBusesExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4AddressExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DHCPEnableStateExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DefaultGatewayExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4NumberOfAddressesExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCalExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCollectionAreaExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMaxPixelBinningExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMulticastEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceConnectionTypeExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceEnableStateExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffsCountExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfNetworkInterfacesExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfPixelsExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchCoatingExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFiberDiameterMicronsExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFilterExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchGratingExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchIDExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSerialNumberExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSlitWidthMicronsExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalDarkPixelRangesExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetPixelBinningExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSaturationExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetScansToAverageExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberMaximumLengthExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffsCountExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureCountExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetThermoElectricTemperatureExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWaveCalExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationModeExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSSIDExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSecurityExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPIntegrationTimeExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLampEnableCommand.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnableCommand.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnabledQuery.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityCommand.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityQuery.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12839 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPMessage.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPQuery.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadI2CMasterBusExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadNumberOfRawSpectraWithMetadataExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrum32AndMetadataExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrum32AndMetadataExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumWithGainExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestBufferedSpectrum32AndMetadata.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestNumberOfBufferedSpectraWithMetadata.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestRawSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRunNetworkInterfaceSelfTestExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSaveNetworkInterfaceConnectionSettingsExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetAcquisitionDelayExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetBoxcarWidthExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetConsecutiveSampleCountExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerAddressExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDataBufferCapacityExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDefaultPixelBinningFactorExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationGbEEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationMACAddressExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetFastBufferingEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionModeExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionOutputVectorExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionValueExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOOutputEnableVectorExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOValueVectorExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DHCPEnableStateExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DefaultGatewayExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCalExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCollectionAreaExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetMulticastEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetNetworkInterfaceEnableStateExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetPixelBinningExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetScansToAverageExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricSetpointExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationModeExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationPassPhraseExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSSIDExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSecurityExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPShutterExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPTransaction.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPTriggerModeExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPWriteI2CMasterBusExchange.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.974012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/hints/
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/hints/OBPControlHint.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/hints/OBPSpectrumHint.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.978012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPAcquisitionDelayProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPContinuousStrobeProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPDHCPServerProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9129 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPDataBufferProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPEthernetConfigurationProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPFastBufferProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    13773 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPGPIOProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPI2CMasterProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9506 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIPv4Protocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIntrospectionProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIrradCalProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol_Ventana.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPMulticastProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPNetworkConfigurationProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPNonlinearityCoeffsProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPOpticalBenchProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPPixelBinningProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPProgrammableSaturationProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPRevisionProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSerialNumberProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPShutterProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12416 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSpectrometerProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSpectrumProcessingProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPStrayLightCoeffsProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPStrobeLampProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPTemperatureProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPThermoElectricProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPWaveCalProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPWifiConfigurationProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OceanBinaryProtocol.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.810013 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.978012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/constants/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/constants/FPGARegisterCodes.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/constants/OpCodes.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.986012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterReadExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterWriteExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGASpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FlameNIRSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/HRFPGASpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/IntegrationTimeExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/JazSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/MayaProSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/NIRQuestSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOI2KSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIIrradCalExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIReadIrradCalExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIWriteIrradCalExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/QESpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadEEPROMSlotExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECQETemperatureExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECTemperatureExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/RequestSpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/StrobeEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TECEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TECQEEnableExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TriggerModeExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/USBFPGASpectrumExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteEEPROMSlotExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECQESetPointExchange.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECSetPointExchange.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.986012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/hints/
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/hints/ControlHint.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/hints/SpectrumHint.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.986012 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/FPGARegisterProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIEEPROMProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIIrradCalProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOISpectrometerProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIStrobeLampProtocol.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOITECProtocol.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.986012 seabreeze-2.7.0/src/seabreeze/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-21 22:40:38.000000 seabreeze-2.7.0/src/seabreeze/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/backends.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.990012 seabreeze-2.7.0/src/seabreeze/cseabreeze/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/cseabreeze/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/cseabreeze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24313 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/cseabreeze/c_seabreeze.pxd
--rw-r--r--   0 runner    (1001) docker     (127)   146429 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/cseabreeze/c_seabreeze_wrapper.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/os_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.990012 seabreeze-2.7.0/src/seabreeze/pyseabreeze/
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    43303 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.994012 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/acquisitiondelay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/continuousstrobe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/databuffer.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/dhcpserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/eeprom.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/ethernetconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/fastbuffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/fpga.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/gpio.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/i2cmaster.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/ipv4.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/irradcal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/lightsource.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/multicast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/networkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/nonlinearity.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/opticalbench.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/pixelbinning.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/rawusb.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/revision.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/shutter.py
--rw-r--r--   0 runner    (1001) docker     (127)    26841 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/spectrometer.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/spectrumprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/straylightcoefficients.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/strobelamp.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/thermoelectric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/wificonfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    25382 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    12950 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/pyseabreeze/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/spectrometers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17529 2024-02-21 22:40:23.000000 seabreeze-2.7.0/src/seabreeze/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.998012 seabreeze-2.7.0/src/seabreeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-02-21 22:40:38.000000 seabreeze-2.7.0/src/seabreeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    84583 2024-02-21 22:40:38.000000 seabreeze-2.7.0/src/seabreeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 22:40:38.000000 seabreeze-2.7.0/src/seabreeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-21 22:40:38.000000 seabreeze-2.7.0/src/seabreeze.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-21 22:40:38.000000 seabreeze-2.7.0/src/seabreeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-21 22:40:38.000000 seabreeze-2.7.0/src/seabreeze.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:40:38.994012 seabreeze-2.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-02-21 22:40:23.000000 seabreeze-2.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-02-21 22:40:23.000000 seabreeze-2.7.0/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-02-21 22:40:23.000000 seabreeze-2.7.0/tests/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-02-21 22:40:23.000000 seabreeze-2.7.0/tests/test_spectrometers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:38.046777 seabreeze-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-01 06:55:26.000000 seabreeze-2.8.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-06-01 06:55:26.000000 seabreeze-2.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-06-01 06:55:26.000000 seabreeze-2.8.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-06-01 06:55:26.000000 seabreeze-2.8.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-06-01 06:55:26.000000 seabreeze-2.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-06-01 06:55:38.046777 seabreeze-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-06-01 06:55:26.000000 seabreeze-2.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.854777 seabreeze-2.8.0/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)    10264 2024-06-01 06:55:26.000000 seabreeze-2.8.0/dev/pretty_print_obp_pcapng.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.854777 seabreeze-2.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-06-01 06:55:26.000000 seabreeze-2.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-06-01 06:55:26.000000 seabreeze-2.8.0/docs/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.854777 seabreeze-2.8.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.854777 seabreeze-2.8.0/docs/source/_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-06-01 06:55:26.000000 seabreeze-2.8.0/docs/source/_extensions/repo_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.858777 seabreeze-2.8.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    36848 2024-06-01 06:55:26.000000 seabreeze-2.8.0/docs/source/_static/overview.png
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-06-01 06:55:26.000000 seabreeze-2.8.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-06-01 06:55:26.000000 seabreeze-2.8.0/docs/source/backend_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-06-01 06:55:26.000000 seabreeze-2.8.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-06-01 06:55:26.000000 seabreeze-2.8.0/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-06-01 06:55:26.000000 seabreeze-2.8.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-06-01 06:55:26.000000 seabreeze-2.8.0/docs/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-06-01 06:55:26.000000 seabreeze-2.8.0/docs/source/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-06-01 06:55:26.000000 seabreeze-2.8.0/docs/source/tldr.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-06-01 06:55:26.000000 seabreeze-2.8.0/docs/source/troubleshoot.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.858777 seabreeze-2.8.0/os_support/
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-06-01 06:55:26.000000 seabreeze-2.8.0/os_support/10-oceanoptics.rules
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-06-01 06:55:26.000000 seabreeze-2.8.0/os_support/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)  7255559 2024-06-01 06:55:26.000000 seabreeze-2.8.0/os_support/windows-driver-files.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-06-01 06:55:26.000000 seabreeze-2.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-06-01 06:55:26.000000 seabreeze-2.8.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-06-01 06:55:26.000000 seabreeze-2.8.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 06:55:38.046777 seabreeze-2.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-06-01 06:55:26.000000 seabreeze-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.850777 seabreeze-2.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.842777 seabreeze-2.8.0/src/libseabreeze/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.834777 seabreeze-2.8.0/src/libseabreeze/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.866777 seabreeze-2.8.0/src/libseabreeze/include/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/DeviceFactory.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/USBEndpointTypes.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.870777 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/AcquisitionDelayFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/ContinuousStrobeFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/DHCPServerFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/DataBufferFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28448 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/DeviceAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/EEPROMFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/EthernetConfigurationFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/FastBufferFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/FeatureAdapterInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/FeatureAdapterTemplate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/FeatureFamilies.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/I2CMasterFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/IPv4FeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/IntrospectionFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/IrradCalFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/LightSourceFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/MulticastFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/NetworkConfigurationFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/NonlinearityCoeffsFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/OpticalBenchFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/PixelBinningFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/ProtocolFamilies.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/RawUSBBusAccessFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/RevisionFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    29520 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPI.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPIConstants.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26268 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPI_Impl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/SerialNumberFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/ShutterFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/SpectrometerFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/SpectrumProcessingFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/StrayLightCoeffsFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/StrobeLampFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/TemperatureFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/ThermoElectricCoolerFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/WifiConfigurationFeatureAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/gpioFeatureAdapter.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.874777 seabreeze-2.8.0/src/libseabreeze/include/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/ByteVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/Data.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/DoubleVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/FloatVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/Log.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/SeaBreeze.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/U32Vector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/UShortVector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/UnitDescriptor.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.874777 seabreeze-2.8.0/src/libseabreeze/include/common/buses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/buses/Bus.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/buses/BusFamilies.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/buses/BusFamily.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/buses/DeviceLocationProberInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/buses/DeviceLocatorInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/buses/TransferHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.874777 seabreeze-2.8.0/src/libseabreeze/include/common/buses/network/
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/buses/network/IPv4NetworkProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/buses/network/IPv4SocketDeviceLocator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/buses/network/TCPIPv4SocketBus.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/buses/network/TCPIPv4SocketTransferHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.874777 seabreeze-2.8.0/src/libseabreeze/include/common/buses/rs232/
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/buses/rs232/RS232DeviceLocator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/buses/rs232/RS232Interface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/buses/rs232/RS232TransferHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.878777 seabreeze-2.8.0/src/libseabreeze/include/common/buses/usb/
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/buses/usb/USBDeviceLocator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/buses/usb/USBInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/buses/usb/USBTransferHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.878777 seabreeze-2.8.0/src/libseabreeze/include/common/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/devices/Device.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.878777 seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/BusConnectException.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/BusException.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/BusTransferException.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/FeatureControlException.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/FeatureException.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/FeatureProtocolNotFoundException.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/IllegalArgumentException.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/NumberFormatException.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/ProtocolBusMismatchException.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/ProtocolException.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/ProtocolFormatException.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/ProtocolTransactionException.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.878777 seabreeze-2.8.0/src/libseabreeze/include/common/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/features/Feature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/features/FeatureFamily.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/features/FeatureImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/globals.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.882777 seabreeze-2.8.0/src/libseabreeze/include/common/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/protocols/Exchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/protocols/Protocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/protocols/ProtocolFamily.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/protocols/ProtocolHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/protocols/ProtocolHint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/protocols/Transaction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/common/protocols/Transfer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.834777 seabreeze-2.8.0/src/libseabreeze/include/native/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.882777 seabreeze-2.8.0/src/libseabreeze/include/native/network/
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/native/network/Inet4Address.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/native/network/Socket.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/native/network/SocketException.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/native/network/SocketTimeoutException.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/native/network/UnknownHostException.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.882777 seabreeze-2.8.0/src/libseabreeze/include/native/network/posix/
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/native/network/posix/NativeSocketPOSIX.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.882777 seabreeze-2.8.0/src/libseabreeze/include/native/network/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/native/network/windows/NativeSocketWindows.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.882777 seabreeze-2.8.0/src/libseabreeze/include/native/rs232/
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/native/rs232/NativeRS232.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/native/rs232/RS232.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.882777 seabreeze-2.8.0/src/libseabreeze/include/native/rs232/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/native/rs232/windows/NativeRS232Windows.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.882777 seabreeze-2.8.0/src/libseabreeze/include/native/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/native/system/NativeSystem.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/native/system/System.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.882777 seabreeze-2.8.0/src/libseabreeze/include/native/usb/
+-rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/native/usb/NativeUSB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/native/usb/USB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/native/usb/USBDiscovery.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.882777 seabreeze-2.8.0/src/libseabreeze/include/native/usb/winusb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/native/usb/winusb/WindowsGUID.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.834777 seabreeze-2.8.0/src/libseabreeze/include/vendors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.842777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.838777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.882777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/network/
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/network/FlameXTCPIPv4.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/network/JazTCPIPv4.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.882777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/rs232/
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/rs232/OOIRS232Interface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.890777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/ApexUSB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameNIRUSB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameXUSB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameXUSBTransferHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR2000PlusUSB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR2000USB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR4000USB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/JazUSB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/Maya2000ProUSB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/Maya2000USB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/MayaLSLUSB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/NIRQuest256USB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/NIRQuest512USB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSB4KSpectrumTransferHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBControlTransferHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBEndpointMaps.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBProductID.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBSpectrumTransferHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBTrivialTransferHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/QE65000USB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/QEProUSB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/STSUSB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/SparkUSB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/TorusUSB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB2000PlusUSB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB2000USB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB4000USB.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/VentanaUSB.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.894777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/Apex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/FlameNIR.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/FlameX.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR2000.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR2000Plus.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR4000.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/Jaz.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/Maya2000.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/Maya2000Pro.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/MayaLSL.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/NIRQuest256.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/NIRQuest512.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/QE65000.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/QEPro.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/STS.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/Spark.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/Torus.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB2000.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB2000Plus.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB4000.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/Ventana.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.842777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.894777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature_FPGA.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/STSAcquisitionDelayFeature.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.894777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature_FPGA.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.894777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/DataBufferFeatureBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/DataBufferFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/FlameXDataBufferFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/QEProDataBufferFeature.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.894777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/dhcp_server/
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/dhcp_server/DHCPServerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/dhcp_server/DHCPServerFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.898777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/NonlinearityEEPROMSlotFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeatureBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_MayaPro.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_NIRQuest.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SerialNumberEEPROMSlotFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/StrayLightEEPROMSlotFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature_QE65000.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.898777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/ethernet_configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.898777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FlameXFastBufferFeature.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.898777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/fpga_register/
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/fpga_register/FPGARegisterFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/fpga_register/FPGARegisterFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.898777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/gpio/
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/gpio/gpioFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/gpio/gpioFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.898777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/i2c_master/
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/i2c_master/i2cMasterFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/i2c_master/i2cMasterFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.898777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/introspection/
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/introspection/IntrospectionFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/introspection/IntrospectionFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.898777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/ipv4/
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/ipv4/IPv4Feature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/ipv4/IPv4FeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.898777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/irradcal/
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/irradcal/IrradCalFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/irradcal/IrradCalFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.902777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/StrobeLampFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/StrobeLampFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/VentanaLightSourceFeature.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.902777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/multicast/
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/multicast/MulticastFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/multicast/MulticastFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.902777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/network_configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.902777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/nonlinearity/
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.902777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/optical_bench/
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/optical_bench/OpticalBenchFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/optical_bench/OpticalBenchFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.902777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/pixel_binning/
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/pixel_binning/PixelBinningFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/pixel_binning/STSPixelBinningFeature.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.902777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/raw_bus_access/
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.902777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/revision/
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/revision/RevisionFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/revision/RevisionFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.902777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/serial_number/
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/serial_number/SerialNumberFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/serial_number/SerialNumberFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.902777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/shutter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/shutter/ShutterFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/shutter/ShutterFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.910777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ApexSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/FlameNIRSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/FlameXSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/GainAdjustedSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR2000PlusSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR2000SpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR4000SpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/JazSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/Maya2000ProSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/Maya2000SpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/MayaLSLSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuest256SpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuest512SpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuestSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureImpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/QE65000SpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/QEProSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/STSSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/SparkSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/SpectrometerTriggerMode.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB2000PlusSpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB2000SpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB4000SpectrometerFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/VentanaSpectrometerFeature.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.910777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrum_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.910777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/stray_light/
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.910777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/temperature/
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/temperature/TemperatureFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/temperature/TemperatureFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.910777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/QEProThermoElectricFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureBase.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricQEFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/VentanaThermoElectricFeature.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.910777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/wavecal/
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/wavecal/WaveCalFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/wavecal/WaveCalFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.910777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/wifi_configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeature.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeatureInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.842777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.918777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/AcquisitionDelayProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ContinuousStrobeProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/DHCPServerProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/DataBufferProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/EEPROMProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/EthernetConfigurationProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/FPGARegisterProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/FastBufferProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/GPIOProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/I2CMasterProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IPv4ProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IntrospectionProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IrradCalProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/LightSourceProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/MulticastProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/NetworkConfigurationProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/NonlinearityCoeffsProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/OpticalBenchProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/PixelBinningProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ProgrammableSaturationProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/RevisionProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SerialNumberProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ShutterProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SpectrometerProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SpectrumProcessingProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/StrayLightCoeffsProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/StrobeLampProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/TemperatureProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ThermoElectricProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/WaveCalProtocolInterface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/WifiConfigurationProtocolInterface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.842777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.918777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)    21778 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/constants/OBPMessageTypes.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.938777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPAddIPv4AddressExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPCommand.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobeEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobePeriodExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferClearExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferRemoveOldestExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDeleteIPv4AddressExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetActivePixelRangesExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetAllTemperaturesExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetBoxcarWidthExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetConsecutiveSampleCountExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerAddressExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCapacityExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferElementCountExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferMaximumCapacityExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDefaultPixelBinningExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetElectricDarkPixelRangesExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationGbEEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationMACAddressExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFastBufferingEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFirmwareRevisionExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionAvailableModesExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionCurrentModeExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionNumberOfPinsExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionOutputVectorExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionValueExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIONumberOfPinsExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOOutputEnableVectorExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOValueVectorExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetHardwareRevisionExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetI2CMasterNumberOfBusesExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4AddressExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DHCPEnableStateExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DefaultGatewayExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4NumberOfAddressesExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCalExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCollectionAreaExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMaxPixelBinningExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMulticastEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceConnectionTypeExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceEnableStateExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffsCountExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfNetworkInterfacesExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfPixelsExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchCoatingExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFiberDiameterMicronsExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFilterExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchGratingExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchIDExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSerialNumberExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSlitWidthMicronsExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalDarkPixelRangesExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetPixelBinningExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSaturationExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetScansToAverageExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberMaximumLengthExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffsCountExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureCountExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetThermoElectricTemperatureExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWaveCalExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationModeExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSSIDExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSecurityExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPIntegrationTimeExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLampEnableCommand.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnableCommand.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnabledQuery.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityCommand.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityQuery.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPMessage.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPQuery.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadI2CMasterBusExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadNumberOfRawSpectraWithMetadataExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrum32AndMetadataExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrum32AndMetadataExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumWithGainExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestBufferedSpectrum32AndMetadataExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestNumberOfBufferedSpectraWithMetadataExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestRawSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRunNetworkInterfaceSelfTestExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSaveNetworkInterfaceConnectionSettingsExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetAcquisitionDelayExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetBoxcarWidthExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetConsecutiveSampleCountExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerAddressExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDataBufferCapacityExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDefaultPixelBinningExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationGbEEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationMACAddressExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetFastBufferingEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionModeExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionOutputVectorExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionValueExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionVectorExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOOutputEnableVectorExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOValueVectorExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DHCPEnableStateExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DefaultGatewayExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCalExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCollectionAreaExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetMulticastEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetNetworkInterfaceEnableStateExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetPixelBinningExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetScansToAverageExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricSetpointExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationModeExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationPassPhraseExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSSIDExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSecurityExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPShutterExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPTransaction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPTriggerModeExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPWriteI2CMasterBusExchange.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.938777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/hints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/hints/OBPControlHint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/hints/OBPSpectrumHint.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.942777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPAcquisitionDelayProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPContinuousStrobeProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPDHCPServerProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPDataBufferProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPEthernetConfigurationProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPFastBufferProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPGPIOProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPI2CMasterProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIPv4Protocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIntrospectionProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIrradCalProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol_Ventana.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPMulticastProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPNetworkConfigurationProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPNonlinearityCoeffsProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPOpticalBenchProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPPixelBinningProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPProgrammableSaturationProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPRevisionProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSerialNumberProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPShutterProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSpectrometerProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSpectrumProcessingProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPStrayLightCoeffsProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPStrobeLampProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPTemperatureProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPThermoElectricProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPWaveCalProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPWifiConfigurationProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OceanBinaryProtocol.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.842777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.942777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/FPGARegisterCodes.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/OpCodes.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/QETECConstants.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.950777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterReadExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterWriteExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGASpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FlameNIRSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/HRFPGASpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/IntegrationTimeExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/JazSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/MayaProSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/NIRQuestSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOI2KSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIIrradCalExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIReadIrradCalExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIWriteIrradCalExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/QESpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadEEPROMSlotExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECQETemperatureExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECTemperatureExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/RequestSpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/StrobeEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TECEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TECQEEnableExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TriggerModeExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/USBFPGASpectrumExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteEEPROMSlotExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECQESetPointExchange.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECSetPointExchange.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.950777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/hints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/hints/ControlHint.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/hints/SpectrumHint.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.950777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/FPGARegisterProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIEEPROMProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIIrradCalProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOISpectrometerProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIStrobeLampProtocol.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOITECProtocol.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.950777 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/utils/Polynomial.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.846777 seabreeze-2.8.0/src/libseabreeze/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.950777 seabreeze-2.8.0/src/libseabreeze/src/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/DeviceFactory.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.958777 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/AcquisitionDelayFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/ContinuousStrobeFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/DHCPServerFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/DataBufferFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    80076 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/DeviceAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/EEPROMFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/EthernetConfigurationFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/FastBufferFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12485 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/FeatureFamilies.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/I2CMasterFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/IPv4FeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5019 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/IntrospectionFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/IrradCalFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/LightSourceFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/MulticastFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/NetworkConfigurationFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/NonlinearityCoeffsFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/OpticalBenchFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/PixelBinningFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/ProtocolFamilies.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/RawUSBBusAccessFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/RevisionFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/SeaBreezeAPI.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    87831 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/SeaBreezeAPI_Impl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/SerialNumberFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/ShutterFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/SpectrometerFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/SpectrumProcessingFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/StrayLightCoeffsFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/StrobeLampFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/TemperatureFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/ThermoElectricCoolerFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/WifiConfigurationFeatureAdapter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/gpioFeatureAdapter.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.958777 seabreeze-2.8.0/src/libseabreeze/src/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/ByteVector.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/Data.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/DoubleVector.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/FloatVector.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/Log.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/U32Vector.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/UShortVector.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/UnitDescriptor.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.958777 seabreeze-2.8.0/src/libseabreeze/src/common/buses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/buses/Bus.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/buses/BusFamilies.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/buses/BusFamily.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/buses/DeviceLocationProberInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/buses/TransferHelper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.958777 seabreeze-2.8.0/src/libseabreeze/src/common/buses/network/
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/buses/network/IPv4NetworkProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/buses/network/IPv4SocketDeviceLocator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/buses/network/TCPIPv4SocketBus.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/buses/network/TCPIPv4SocketTransferHelper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.962777 seabreeze-2.8.0/src/libseabreeze/src/common/buses/rs232/
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/buses/rs232/RS232DeviceLocator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/buses/rs232/RS232Interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/buses/rs232/RS232TransferHelper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.962777 seabreeze-2.8.0/src/libseabreeze/src/common/buses/usb/
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/buses/usb/USBDeviceLocator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/buses/usb/USBInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/buses/usb/USBTransferHelper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.962777 seabreeze-2.8.0/src/libseabreeze/src/common/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/devices/Device.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.962777 seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/BusConnectException.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/BusException.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/BusTransferException.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/FeatureControlException.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/FeatureException.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/FeatureProtocolNotFoundException.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/IllegalArgumentException.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/NumberFormatException.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/ProtocolBusMismatchException.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/ProtocolException.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/ProtocolFormatException.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/ProtocolTransactionException.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.962777 seabreeze-2.8.0/src/libseabreeze/src/common/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/features/FeatureFamily.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/features/FeatureImpl.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.966777 seabreeze-2.8.0/src/libseabreeze/src/common/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/protocols/Exchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/protocols/Protocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/protocols/ProtocolFamily.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/protocols/ProtocolHelper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/protocols/ProtocolHint.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/protocols/Transaction.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/common/protocols/Transfer.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.846777 seabreeze-2.8.0/src/libseabreeze/src/native/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.966777 seabreeze-2.8.0/src/libseabreeze/src/native/network/
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/native/network/Inet4Address.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/native/network/SocketException.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/native/network/SocketTimeoutException.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/native/network/UnknownHostException.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.966777 seabreeze-2.8.0/src/libseabreeze/src/native/network/posix/
+-rw-r--r--   0 runner    (1001) docker     (127)     7271 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/native/network/posix/NativeSocketPOSIX.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.966777 seabreeze-2.8.0/src/libseabreeze/src/native/network/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/native/network/windows/NativeSocketWindows.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.966777 seabreeze-2.8.0/src/libseabreeze/src/native/rs232/
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/native/rs232/RS232.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.966777 seabreeze-2.8.0/src/libseabreeze/src/native/rs232/posix/
+-rw-r--r--   0 runner    (1001) docker     (127)    12360 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/native/rs232/posix/NativeRS232POSIX.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.966777 seabreeze-2.8.0/src/libseabreeze/src/native/rs232/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)     7796 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/native/rs232/windows/NativeRS232Windows.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.966777 seabreeze-2.8.0/src/libseabreeze/src/native/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/native/system/System.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.966777 seabreeze-2.8.0/src/libseabreeze/src/native/system/posix/
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/native/system/posix/NativeSystemPOSIX.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.966777 seabreeze-2.8.0/src/libseabreeze/src/native/system/windows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/native/system/windows/NativeSystemWindows.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.966777 seabreeze-2.8.0/src/libseabreeze/src/native/usb/
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/native/usb/USB.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/native/usb/USBDiscovery.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.966777 seabreeze-2.8.0/src/libseabreeze/src/native/usb/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)    22561 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/native/usb/linux/NativeUSBLinux.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.966777 seabreeze-2.8.0/src/libseabreeze/src/native/usb/osx/
+-rw-r--r--   0 runner    (1001) docker     (127)    38021 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/native/usb/osx/NativeUSBMacOSX.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.970777 seabreeze-2.8.0/src/libseabreeze/src/native/usb/winusb/
+-rw-r--r--   0 runner    (1001) docker     (127)    28911 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/native/usb/winusb/NativeUSBWinUSB.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.846777 seabreeze-2.8.0/src/libseabreeze/src/vendors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.850777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.846777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.970777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/network/
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/network/FlameXTCPIPv4.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/network/JazTCPIPv4.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.970777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/rs232/
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/rs232/OOIRS232Interface.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.974777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/ApexUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameNIRUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameXUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameXUSBTransferHelper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR2000PlusUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR2000USB.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR4000USB.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/JazUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/Maya2000ProUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/Maya2000USB.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/MayaLSLUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/NIRQuest256USB.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/NIRQuest512USB.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSB4KSpectrumTransferHelper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBControlTransferHelper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBEndpointMaps.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBSpectrumTransferHelper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBTrivialTransferHelper.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/QE65000USB.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/QEProUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/STSUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/SparkUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/TorusUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB2000PlusUSB.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB2000USB.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB4000USB.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/VentanaUSB.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.978777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/Apex.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/FlameNIR.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/FlameX.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR2000.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR2000Plus.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR4000.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/Jaz.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/Maya2000.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/Maya2000Pro.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/MayaLSL.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/NIRQuest256.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/NIRQuest512.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/QE65000.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/QEPro.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/STS.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/Spark.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/Torus.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB2000.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB2000Plus.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB4000.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7724 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/Ventana.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.850777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.978777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature_FPGA.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/STSAcquisitionDelayFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.978777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/continuous_strobe/
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature_FPGA.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.978777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/
+-rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/DataBufferFeatureBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/FlameXDataBufferFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/QEProDataBufferFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.978777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/dhcp_server/
+-rw-r--r--   0 runner    (1001) docker     (127)     6430 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/dhcp_server/DHCPServerFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.982777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/NonlinearityEEPROMSlotFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeatureBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_MayaPro.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_NIRQuest.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SerialNumberEEPROMSlotFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/StrayLightEEPROMSlotFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature_QE65000.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.982777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/ethernet_configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.982777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/fast_buffer/
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/fast_buffer/FlameXFastBufferFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.982777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/fpga_register/
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/fpga_register/FPGARegisterFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.982777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/gpio/
+-rw-r--r--   0 runner    (1001) docker     (127)    13793 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/gpio/gpioFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.982777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/i2c_master/
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/i2c_master/i2cFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.982777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/introspection/
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/introspection/IntrospectionFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.982777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/ipv4/
+-rw-r--r--   0 runner    (1001) docker     (127)     9822 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/ipv4/IPv4Feature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.982777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/irradcal/
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/irradcal/IrradCalFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.982777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/
+-rw-r--r--   0 runner    (1001) docker     (127)    14844 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/LightSourceFeatureBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/LightSourceFeatureImpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/StrobeLampFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/VentanaLightSourceFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.982777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/multicast/
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/multicast/MulticastFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.982777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/network_configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.986777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/nonlinearity/
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.986777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/optical_bench/
+-rw-r--r--   0 runner    (1001) docker     (127)     9817 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/optical_bench/OpticalBenchFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.986777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/pixel_binning/
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/pixel_binning/PixelBinningFeatureInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/pixel_binning/STSPixelBinningFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.986777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/raw_bus_access/
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.986777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/revision/
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/revision/RevisionFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.986777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/serial_number/
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/serial_number/SerialNumberFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.986777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/shutter/
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/shutter/ShutterFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.990777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ApexSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/FlameNIRSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/FlameXSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/GainAdjustedSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR2000PlusSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR2000SpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR4000SpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/JazSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/Maya2000ProSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/Maya2000SpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/MayaLSLSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuest256SpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuest512SpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuestSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14571 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureImpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/QE65000SpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/QEProSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/STSSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/SparkSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/SpectrometerTriggerMode.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB2000PlusSpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB2000SpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB4000SpectrometerFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/VentanaSpectrometerFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.990777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrum_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.990777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/stray_light/
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.990777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/temperature/
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/temperature/TemperatureFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.990777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/QEProThermoElectricFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureBase.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/ThermoElectricQEFeature.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/VentanaThermoElectricFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.990777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/wavecal/
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/wavecal/WaveCalFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.990777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/wifi_configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     9640 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeature.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.850777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.998777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/AcquisitionDelayProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ContinuousStrobeProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/DHCPServerProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/DataBufferProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/EEPROMProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/EthernetConfigurationProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/FPGARegisterProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/FastBufferProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/GPIOProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/I2CMasterProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IPv4ProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IntrospectionProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IrradCalProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/LightSourceProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/MulticastProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/NetworkConfigurationProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/NonlinearityCoeffsProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/OpticalBenchProtocolInteface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/PixelBinningProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ProgrammableSaturationProtocolInteface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/RevisionProtocolInteface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SerialNumberProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ShutterProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SpectrometerProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SpectrumProcessingProtocolInteface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/StrayLightCoeffsProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/StrobeLampProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/TemperatureProtocolInteface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ThermoElectricProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/WaveCalProtocolInterface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/WifiConfigurationProtocolInterface.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.850777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:38.022777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPAddIPv4AddressExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPCommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobeEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobePeriodExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferClearExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferRemoveOldestExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDeleteIPv4AddressExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetActivePixelRangesExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetAllTemperaturesExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetBoxcarWidthExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetConsecutiveSampleCountExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerAddressExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCapacityExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCountExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferMaximumCapacityExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDefaultPixelBinningExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetElectricDarkPixelRangesExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationGbEEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationMACAddressExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFastBufferingEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFirmwareRevisionExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionAvailableModesExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionCurrentModeExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionNumberOfPinsExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionOutputVectorExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionValueExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIONumberOfPinsExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOOutputEnableVectorExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOValueVectorExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetHardwareRevisionExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetI2CMasterNumberOfBusesExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4AddressExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DHCPEnableStateExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DefaultGatewayExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4NumberOfAddressesExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCalExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCollectionAreaExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMaxPixelBinningExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMulticastEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceConnectionTypeExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceEnableStateExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffsCountExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfNetworkInterfacesExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfPixelsExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchCoatingExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFiberDiameterMicronsExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFilterExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchGratingExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchIDExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSerialNumberExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSlitWidthMicronsExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalDarkPixelRangesExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetPixelBinningExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSaturationExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetScansToAverageExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberMaximumLengthExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffsCountExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureCountExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetThermoElectricTemperatureExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWaveCalExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationModeExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSSIDExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSecurityExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPIntegrationTimeExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLampEnableCommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnableCommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnabledQuery.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityCommand.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityQuery.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12839 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPMessage.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPQuery.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadI2CMasterBusExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadNumberOfRawSpectraWithMetadataExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrum32AndMetadataExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrum32AndMetadataExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumWithGainExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestBufferedSpectrum32AndMetadata.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestNumberOfBufferedSpectraWithMetadata.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestRawSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRunNetworkInterfaceSelfTestExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSaveNetworkInterfaceConnectionSettingsExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetAcquisitionDelayExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetBoxcarWidthExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetConsecutiveSampleCountExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerAddressExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDataBufferCapacityExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDefaultPixelBinningFactorExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationGbEEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationMACAddressExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetFastBufferingEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionModeExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionOutputVectorExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionValueExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOOutputEnableVectorExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOValueVectorExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DHCPEnableStateExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DefaultGatewayExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCalExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCollectionAreaExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetMulticastEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetNetworkInterfaceEnableStateExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetPixelBinningExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetScansToAverageExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricSetpointExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationModeExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationPassPhraseExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSSIDExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSecurityExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPShutterExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPTransaction.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPTriggerModeExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPWriteI2CMasterBusExchange.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:38.022777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/hints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/hints/OBPControlHint.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/hints/OBPSpectrumHint.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:38.026777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPAcquisitionDelayProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPContinuousStrobeProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPDHCPServerProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9129 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPDataBufferProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPEthernetConfigurationProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPFastBufferProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    13773 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPGPIOProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPI2CMasterProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9506 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIPv4Protocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIntrospectionProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIrradCalProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol_Ventana.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPMulticastProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPNetworkConfigurationProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPNonlinearityCoeffsProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPOpticalBenchProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6918 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPPixelBinningProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPProgrammableSaturationProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPRevisionProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSerialNumberProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPShutterProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12416 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSpectrometerProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSpectrumProcessingProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPStrayLightCoeffsProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPStrobeLampProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPTemperatureProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPThermoElectricProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPWaveCalProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8531 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPWifiConfigurationProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OceanBinaryProtocol.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:37.850777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:38.026777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/constants/FPGARegisterCodes.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/constants/OpCodes.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:38.034777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterReadExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterWriteExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGASpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FlameNIRSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/HRFPGASpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/IntegrationTimeExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/JazSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/MayaProSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/NIRQuestSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOI2KSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIIrradCalExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIReadIrradCalExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIWriteIrradCalExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/QESpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadEEPROMSlotExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECQETemperatureExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECTemperatureExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/RequestSpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/StrobeEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TECEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TECQEEnableExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TriggerModeExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/USBFPGASpectrumExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteEEPROMSlotExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECQESetPointExchange.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECSetPointExchange.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:38.034777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/hints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/hints/ControlHint.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/hints/SpectrumHint.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:38.034777 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/FPGARegisterProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIEEPROMProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIIrradCalProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOISpectrometerProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIStrobeLampProtocol.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOITECProtocol.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:38.034777 seabreeze-2.8.0/src/seabreeze/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-01 06:55:37.000000 seabreeze-2.8.0/src/seabreeze/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/backends.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:38.038777 seabreeze-2.8.0/src/seabreeze/cseabreeze/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/cseabreeze/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/cseabreeze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24313 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/cseabreeze/c_seabreeze.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)   146429 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/cseabreeze/c_seabreeze_wrapper.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/os_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:38.038777 seabreeze-2.8.0/src/seabreeze/pyseabreeze/
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44742 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:38.046777 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/acquisitiondelay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/continuousstrobe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/databuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/dhcpserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/ethernetconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/fastbuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/fpga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/i2cmaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/irradcal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/lightsource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/multicast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/networkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/nonlinearity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/opticalbench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/pixelbinning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/rawusb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/shutter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28814 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/spectrometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/spectrumprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/straylightcoefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/strobelamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/thermoelectric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/wificonfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25382 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12950 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/pyseabreeze/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/spectrometers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17529 2024-06-01 06:55:26.000000 seabreeze-2.8.0/src/seabreeze/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:38.046777 seabreeze-2.8.0/src/seabreeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-06-01 06:55:37.000000 seabreeze-2.8.0/src/seabreeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    84583 2024-06-01 06:55:37.000000 seabreeze-2.8.0/src/seabreeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 06:55:37.000000 seabreeze-2.8.0/src/seabreeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-01 06:55:37.000000 seabreeze-2.8.0/src/seabreeze.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-06-01 06:55:37.000000 seabreeze-2.8.0/src/seabreeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 06:55:37.000000 seabreeze-2.8.0/src/seabreeze.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:55:38.046777 seabreeze-2.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-06-01 06:55:26.000000 seabreeze-2.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-06-01 06:55:26.000000 seabreeze-2.8.0/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-06-01 06:55:26.000000 seabreeze-2.8.0/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-06-01 06:55:26.000000 seabreeze-2.8.0/tests/test_spectrometers.py
```

### Comparing `seabreeze-2.7.0/.pre-commit-config.yaml` & `seabreeze-2.8.0/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 default_language_version:
     python: python3.10
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
     -   id: trailing-whitespace
     -   id: end-of-file-fixer
     -   id: check-yaml
     -   id: check-added-large-files
 -   repo: https://github.com/psf/black
-    rev: '24.2.0'
+    rev: '24.4.2'
     hooks:
     -   id: black
         language_version: python3
 -   repo: https://github.com/pycqa/isort
     rev: 5.13.2
     hooks:
     -   id: isort
@@ -24,22 +24,22 @@
     hooks:
     -   id: flake8
         additional_dependencies:
         -    flake8-typing-imports==1.14.0
         language_version: python3
         exclude: "^(build|docs|tests|setup.py)"
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: 'v1.8.0'
+    rev: 'v1.10.0'
     hooks:
     -   id: mypy
         additional_dependencies: [numpy<1.25, pyusb>=1.0]
         exclude: "^(build|docs|tests|dev|setup.py)"
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.15.1
+    rev: v3.15.2
     hooks:
     -   id: pyupgrade
         args: [--py38-plus]
 -   repo: https://github.com/MarcoGorelli/cython-lint
-    rev: v0.16.0
+    rev: v0.16.2
     hooks:
     -   id: cython-lint
     -   id: double-quote-cython-strings
```

### Comparing `seabreeze-2.7.0/CHANGELOG.md` & `seabreeze-2.8.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 | *psb*  | refers to `seabreeze.pyseabreeze`   |
 | *spec* | refers to `seabreeze.spectrometers` |
 
 
 ## [Unreleased]
 ...
 
+## [2.8.0] - 2024-06-01
+### Added
+- *psb* added support for HR2 spectrometer (pyseabreeze backend) (thanks @gabrielbenedikt)
+- *psb* added support for HR4 spectrometer (pyseabreeze backend) (thanks @MicheleCotrufo)
+
 ## [2.7.0] - 2024-02-21
 ### Added
 - *csb* added support for get_fast_buffer_spectrum() (cseabreeze backend) (thanks @padalev)
 
 ## [2.6.0] - 2024-01-24
 ### Changed
 - *psb* Use currently set integration time for timeout instead of the maximum integration time.
@@ -225,15 +230,16 @@
 ## [0.5.3] - 2016-02-16
 ### Added
 - oldest version I'll go back to in this changelog
 
 ### Changed
 - Don't require numpy during build of cseabreeze cython extension
 
-[Unreleased]: https://github.com/ap--/python-seabreeze/compare/v2.7.0...HEAD
+[Unreleased]: https://github.com/ap--/python-seabreeze/compare/v2.8.0...HEAD
+[2.8.0]: https://github.com/ap--/python-seabreeze/compare/v2.7.0...v2.8.0
 [2.7.0]: https://github.com/ap--/python-seabreeze/compare/v2.6.0...v2.7.0
 [2.6.0]: https://github.com/ap--/python-seabreeze/compare/v2.5.0...v2.6.0
 [2.5.0]: https://github.com/ap--/python-seabreeze/compare/v2.4.0...v2.5.0
 [2.4.0]: https://github.com/ap--/python-seabreeze/compare/v2.3.0...v2.4.0
 [2.3.0]: https://github.com/ap--/python-seabreeze/compare/v2.2.0...v2.3.0
 [2.2.0]: https://github.com/ap--/python-seabreeze/compare/v2.1.0...v2.2.0
 [2.1.0]: https://github.com/ap--/python-seabreeze/compare/v2.0.3...v2.1.0
```

### Comparing `seabreeze-2.7.0/LICENSE.md` & `seabreeze-2.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/PKG-INFO` & `seabreeze-2.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seabreeze
-Version: 2.7.0
+Version: 2.8.0
 Summary: Python interface module for Ocean Optics spectrometers. This software is not associated with Ocean Optics. Use it at your own risk.
 Home-page: https://github.com/ap--/python-seabreeze
 Author: Andreas Poehlmann
 Author-email: andreas@poehlmann.io
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -62,14 +62,24 @@
 
 ```bash
 # via conda
 conda install -c conda-forge seabreeze
 seabreeze_os_setup
 ```
 
+### Using the backend pyseabreeze in Windows
+
+The backend pyseabreeze requires the libraries pyusb and libusb
+```bash
+# via pypi
+pip install seabreeze[pyseabreeze]  # this ensures installation of pyusb
+```
+Additionally, you might need to manually install libusb1. Go here https://libusb.info/, Downloads -> Latest Windows Binaries. In the zip file, enter either the folder MinGW64/dll or MinGW32/dll (depending on your OS). Copy the file `libusb-1.0.dll` into `C:\Windows\System32`.
+
+
 ## Usage
 
 The following example shows how simple it is to acquire a spectrum with
 python-seabreeze through the model independent _Spectrometer_ class. For a more
 detailed description read the [documentation](https://python-seabreeze.readthedocs.io/en/latest/):
 
 ```python
@@ -114,14 +124,16 @@
 | USB4000      |     x      |            x             |
 | USB650       |            | ap--/python-seabreeze#47 |
 | SPARK        |     x      |            x             |
 | ADC1000      |            |            x             |
 | SR2          |            |            x             |
 | SR4          |            |            x             |
 | SR6          |            |            x             |
+| HR2          |            |            x             |
+| HR4          |            |            x             |
 | ST-VIS       |            |            x             |
 
 
 ## Known Issues
 
 - USB2000 spectrometers cause `Data transfer error` due to old firmware [Issue #48](https://github.com/ap--/python-seabreeze/issues/48)
 - USB650 not supported [Issue #47](https://github.com/ap--/python-seabreeze/issues/47)
```

### Comparing `seabreeze-2.7.0/README.md` & `seabreeze-2.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,24 @@
 
 ```bash
 # via conda
 conda install -c conda-forge seabreeze
 seabreeze_os_setup
 ```
 
+### Using the backend pyseabreeze in Windows
+
+The backend pyseabreeze requires the libraries pyusb and libusb
+```bash
+# via pypi
+pip install seabreeze[pyseabreeze]  # this ensures installation of pyusb
+```
+Additionally, you might need to manually install libusb1. Go here https://libusb.info/, Downloads -> Latest Windows Binaries. In the zip file, enter either the folder MinGW64/dll or MinGW32/dll (depending on your OS). Copy the file `libusb-1.0.dll` into `C:\Windows\System32`.
+
+
 ## Usage
 
 The following example shows how simple it is to acquire a spectrum with
 python-seabreeze through the model independent _Spectrometer_ class. For a more
 detailed description read the [documentation](https://python-seabreeze.readthedocs.io/en/latest/):
 
 ```python
@@ -89,14 +99,16 @@
 | USB4000      |     x      |            x             |
 | USB650       |            | ap--/python-seabreeze#47 |
 | SPARK        |     x      |            x             |
 | ADC1000      |            |            x             |
 | SR2          |            |            x             |
 | SR4          |            |            x             |
 | SR6          |            |            x             |
+| HR2          |            |            x             |
+| HR4          |            |            x             |
 | ST-VIS       |            |            x             |
 
 
 ## Known Issues
 
 - USB2000 spectrometers cause `Data transfer error` due to old firmware [Issue #48](https://github.com/ap--/python-seabreeze/issues/48)
 - USB650 not supported [Issue #47](https://github.com/ap--/python-seabreeze/issues/47)
```

### Comparing `seabreeze-2.7.0/dev/pretty_print_obp_pcapng.py` & `seabreeze-2.8.0/dev/pretty_print_obp_pcapng.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/docs/Makefile` & `seabreeze-2.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/docs/source/_extensions/repo_file.py` & `seabreeze-2.8.0/docs/source/_extensions/repo_file.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/docs/source/_static/overview.png` & `seabreeze-2.8.0/docs/source/_static/overview.png`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/docs/source/api.rst` & `seabreeze-2.8.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/docs/source/backend_api.rst` & `seabreeze-2.8.0/docs/source/backend_api.rst`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/docs/source/conf.py` & `seabreeze-2.8.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/docs/source/contributing.rst` & `seabreeze-2.8.0/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/docs/source/index.rst` & `seabreeze-2.8.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/docs/source/install.rst` & `seabreeze-2.8.0/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/docs/source/quickstart.rst` & `seabreeze-2.8.0/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/docs/source/tldr.rst` & `seabreeze-2.8.0/docs/source/tldr.rst`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/docs/source/troubleshoot.rst` & `seabreeze-2.8.0/docs/source/troubleshoot.rst`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/os_support/10-oceanoptics.rules` & `seabreeze-2.8.0/os_support/10-oceanoptics.rules`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # udev rules file for Ocean Optics, Inc. spectrometers
 # ====================================================
 #
-# version: 2.6
-# updated: 2024-01-24
+# version: 2.8
+# updated: 2024-06-01
 # maintainer: Andreas Poehlmann <andreas@poehlmann.io>
 #
 # [info] Previous versions are missing this header.
 #
 # Ships with [python-seabreeze](https://github.com/ap--/python-seabreeze/)
 # Only USB spectrometers are supported. When using the newest version (1.0+)
 # of python-seabreeze you can install the rules via running:
 #
 #   $ seabreeze_os_setup
 #
 # Changes:
+# - [2.8] added support for HR4 spectrometer
+# - [2.7] added support for HR2 spectrometer
 # - [2.6] added support for SR6 spectrometer
 # - [2.5] added support for SR2 spectrometer
 # - [2.4] added support for SR4 spectrometer
 # - added support for HDX spectrometer
 # - added support for QE-PRO class of OceanOptics spectrometers
 # - set MODE instead of group (Fedora doesn't use `plugdev`)
 # - match parent SUBSYSTEMS for compatibility with older udev versions
@@ -85,15 +87,19 @@
 ATTR{idVendor}=="0547", ATTR{idProduct}=="2235", SYMLINK+="ezUSB-FX-%n", MODE:="0666"
 # unprogrammed EzUSB-FX2
 ATTR{idVendor}=="04b4", ATTR{idProduct}=="8613", SYMLINK+="ezUSB-FX2-%n", MODE:="0666"
 # Ocean Insight Inc. HDX spectrometer
 ATTR{idVendor}=="2457", ATTR{idProduct}=="2003", SYMLINK+="oceanhdx-%n", MODE:="0666"
 # Ocean Insight Inc. ST spectrometer
 ATTR{idVendor}=="0999", ATTR{idProduct}=="1000", SYMLINK+="st-%n", MODE:="0666"
-# Ocean Insight Inc. SR4 spectrometer
+# Ocean Insight Inc. SR2 spectrometer
 ATTR{idVendor}=="0999", ATTR{idProduct}=="1001", SYMLINK+="sr2-%n", MODE:="0666"
 # Ocean Insight Inc. SR4 spectrometer
 ATTR{idVendor}=="0999", ATTR{idProduct}=="1002", SYMLINK+="sr4-%n", MODE:="0666"
 # Ocean Insight Inc. SR6 Spectrometer
 ATTR{idVendor}=="0999", ATTR{idProduct}=="1005", SYMLINK+="sr6-%n", MODE:="0666"
+# Ocean Insight Inc. HR2 Spectrometer
+ATTR{idVendor}=="0999", ATTR{idProduct}=="1003", SYMLINK+="hr2-%n", MODE:="0666"
+# Ocean Insight Inc. HR4 Spectrometer
+ATTR{idVendor}=="0999", ATTR{idProduct}=="1004", SYMLINK+="hr4-%n", MODE:="0666"
 
 LABEL="oceanoptics_rules_end"
```

### Comparing `seabreeze-2.7.0/os_support/readme.md` & `seabreeze-2.8.0/os_support/readme.md`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/os_support/windows-driver-files.zip` & `seabreeze-2.8.0/os_support/windows-driver-files.zip`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/pyproject.toml` & `seabreeze-2.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/setup.py` & `seabreeze-2.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/DeviceFactory.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/DeviceFactory.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/USBEndpointTypes.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/USBEndpointTypes.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/AcquisitionDelayFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/AcquisitionDelayFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/ContinuousStrobeFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/ContinuousStrobeFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/DHCPServerFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/DHCPServerFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/DataBufferFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/DataBufferFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/DeviceAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/DeviceAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/EEPROMFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/EEPROMFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/EthernetConfigurationFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/EthernetConfigurationFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/FastBufferFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/FastBufferFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/FeatureAdapterInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/FeatureAdapterInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/FeatureAdapterTemplate.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/FeatureAdapterTemplate.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/FeatureFamilies.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/FeatureFamilies.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/I2CMasterFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/I2CMasterFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/IPv4FeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/IPv4FeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/IntrospectionFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/IntrospectionFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/IrradCalFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/IrradCalFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/LightSourceFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/LightSourceFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/MulticastFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/MulticastFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/NetworkConfigurationFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/NetworkConfigurationFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/NonlinearityCoeffsFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/NonlinearityCoeffsFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/OpticalBenchFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/OpticalBenchFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/PixelBinningFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/PixelBinningFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/ProtocolFamilies.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/ProtocolFamilies.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/RawUSBBusAccessFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/RawUSBBusAccessFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/RevisionFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/RevisionFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPI.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPI.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPIConstants.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPIConstants.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPI_Impl.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/SeaBreezeAPI_Impl.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/SerialNumberFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/SerialNumberFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/ShutterFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/ShutterFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/SpectrometerFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/SpectrometerFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/SpectrumProcessingFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/SpectrumProcessingFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/StrayLightCoeffsFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/StrayLightCoeffsFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/StrobeLampFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/StrobeLampFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/TemperatureFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/TemperatureFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/ThermoElectricCoolerFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/ThermoElectricCoolerFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/WifiConfigurationFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/WifiConfigurationFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/api/seabreezeapi/gpioFeatureAdapter.h` & `seabreeze-2.8.0/src/libseabreeze/include/api/seabreezeapi/gpioFeatureAdapter.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/ByteVector.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/ByteVector.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/Data.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/Data.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/DoubleVector.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/DoubleVector.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/FloatVector.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/FloatVector.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/Log.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/Log.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/SeaBreeze.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/SeaBreeze.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/U32Vector.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/U32Vector.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/UShortVector.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/UShortVector.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/UnitDescriptor.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/UnitDescriptor.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/buses/Bus.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/buses/Bus.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/buses/BusFamilies.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/buses/BusFamilies.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/buses/BusFamily.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/buses/BusFamily.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/buses/DeviceLocationProberInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/buses/DeviceLocationProberInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/buses/DeviceLocatorInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/buses/DeviceLocatorInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/buses/TransferHelper.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/buses/TransferHelper.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/buses/network/IPv4NetworkProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/buses/network/IPv4NetworkProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/buses/network/IPv4SocketDeviceLocator.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/buses/network/IPv4SocketDeviceLocator.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/buses/network/TCPIPv4SocketBus.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/buses/network/TCPIPv4SocketBus.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/buses/network/TCPIPv4SocketTransferHelper.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/buses/network/TCPIPv4SocketTransferHelper.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/buses/rs232/RS232DeviceLocator.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/buses/rs232/RS232DeviceLocator.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/buses/rs232/RS232Interface.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/buses/rs232/RS232Interface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/buses/rs232/RS232TransferHelper.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/buses/rs232/RS232TransferHelper.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/buses/usb/USBDeviceLocator.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/buses/usb/USBDeviceLocator.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/buses/usb/USBInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/buses/usb/USBInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/buses/usb/USBTransferHelper.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/buses/usb/USBTransferHelper.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/devices/Device.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/devices/Device.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/BusConnectException.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/BusConnectException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/BusException.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/BusException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/BusTransferException.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/BusTransferException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/FeatureControlException.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/FeatureControlException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/FeatureException.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/FeatureException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/FeatureProtocolNotFoundException.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/FeatureProtocolNotFoundException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/IllegalArgumentException.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/IllegalArgumentException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/NumberFormatException.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/NumberFormatException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/ProtocolBusMismatchException.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/ProtocolBusMismatchException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/ProtocolException.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/ProtocolException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/ProtocolFormatException.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/ProtocolFormatException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/exceptions/ProtocolTransactionException.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/exceptions/ProtocolTransactionException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/features/Feature.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/features/Feature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/features/FeatureFamily.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/features/FeatureFamily.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/features/FeatureImpl.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/features/FeatureImpl.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/globals.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/globals.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/protocols/Exchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/protocols/Exchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/protocols/Protocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/protocols/Protocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/protocols/ProtocolFamily.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/protocols/ProtocolFamily.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/protocols/ProtocolHelper.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/protocols/ProtocolHelper.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/protocols/ProtocolHint.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/protocols/ProtocolHint.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/protocols/Transaction.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/protocols/Transaction.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/common/protocols/Transfer.h` & `seabreeze-2.8.0/src/libseabreeze/include/common/protocols/Transfer.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/native/network/Inet4Address.h` & `seabreeze-2.8.0/src/libseabreeze/include/native/network/Inet4Address.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/native/network/Socket.h` & `seabreeze-2.8.0/src/libseabreeze/include/native/network/Socket.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/native/network/SocketException.h` & `seabreeze-2.8.0/src/libseabreeze/include/native/network/SocketException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/native/network/SocketTimeoutException.h` & `seabreeze-2.8.0/src/libseabreeze/include/native/network/SocketTimeoutException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/native/network/UnknownHostException.h` & `seabreeze-2.8.0/src/libseabreeze/include/native/network/UnknownHostException.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/native/network/posix/NativeSocketPOSIX.h` & `seabreeze-2.8.0/src/libseabreeze/include/native/network/posix/NativeSocketPOSIX.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/native/network/windows/NativeSocketWindows.h` & `seabreeze-2.8.0/src/libseabreeze/include/native/network/windows/NativeSocketWindows.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/native/rs232/NativeRS232.h` & `seabreeze-2.8.0/src/libseabreeze/include/native/rs232/NativeRS232.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/native/rs232/RS232.h` & `seabreeze-2.8.0/src/libseabreeze/include/native/rs232/RS232.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/native/rs232/windows/NativeRS232Windows.h` & `seabreeze-2.8.0/src/libseabreeze/include/native/rs232/windows/NativeRS232Windows.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/native/system/NativeSystem.h` & `seabreeze-2.8.0/src/libseabreeze/include/native/system/NativeSystem.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/native/system/System.h` & `seabreeze-2.8.0/src/libseabreeze/include/native/system/System.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/native/usb/NativeUSB.h` & `seabreeze-2.8.0/src/libseabreeze/include/native/usb/NativeUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/native/usb/USB.h` & `seabreeze-2.8.0/src/libseabreeze/include/native/usb/USB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/native/usb/USBDiscovery.h` & `seabreeze-2.8.0/src/libseabreeze/include/native/usb/USBDiscovery.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/native/usb/winusb/WindowsGUID.h` & `seabreeze-2.8.0/src/libseabreeze/include/native/usb/winusb/WindowsGUID.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/network/FlameXTCPIPv4.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/network/FlameXTCPIPv4.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/network/JazTCPIPv4.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/network/JazTCPIPv4.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/rs232/OOIRS232Interface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/rs232/OOIRS232Interface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/ApexUSB.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/ApexUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameNIRUSB.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameNIRUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameXUSB.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameXUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameXUSBTransferHelper.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/FlameXUSBTransferHelper.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR2000PlusUSB.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR2000PlusUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR2000USB.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR2000USB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR4000USB.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/HR4000USB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/JazUSB.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/JazUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/Maya2000ProUSB.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/Maya2000ProUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/Maya2000USB.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/Maya2000USB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/MayaLSLUSB.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/MayaLSLUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/NIRQuest256USB.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/NIRQuest256USB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/NIRQuest512USB.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/NIRQuest512USB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSB4KSpectrumTransferHelper.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSB4KSpectrumTransferHelper.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBControlTransferHelper.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBControlTransferHelper.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBEndpointMaps.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBEndpointMaps.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBProductID.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBProductID.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBSpectrumTransferHelper.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBSpectrumTransferHelper.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBTrivialTransferHelper.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/OOIUSBTrivialTransferHelper.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/QE65000USB.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/QE65000USB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/QEProUSB.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/QEProUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/STSUSB.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/STSUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/SparkUSB.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/SparkUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/TorusUSB.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/TorusUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB2000PlusUSB.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB2000PlusUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB2000USB.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB2000USB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB4000USB.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/USB4000USB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/VentanaUSB.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/buses/usb/VentanaUSB.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/Apex.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/Apex.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/FlameNIR.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/FlameNIR.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/FlameX.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/FlameX.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR2000.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR2000.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR2000Plus.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR2000Plus.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR4000.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/HR4000.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/Jaz.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/Jaz.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/Maya2000.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/Maya2000.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/Maya2000Pro.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/Maya2000Pro.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/MayaLSL.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/MayaLSL.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/NIRQuest256.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/NIRQuest256.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/NIRQuest512.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/NIRQuest512.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/QE65000.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/QE65000.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/QEPro.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/QEPro.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/STS.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/STS.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/Spark.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/Spark.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/Torus.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/Torus.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB2000.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB2000.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB2000Plus.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB2000Plus.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB4000.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/USB4000.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/devices/Ventana.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/devices/Ventana.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature_FPGA.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature_FPGA.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/STSAcquisitionDelayFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/acquisition_delay/STSAcquisitionDelayFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature_FPGA.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature_FPGA.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/DataBufferFeatureBase.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/DataBufferFeatureBase.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/DataBufferFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/DataBufferFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/FlameXDataBufferFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/FlameXDataBufferFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/QEProDataBufferFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/data_buffer/QEProDataBufferFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/dhcp_server/DHCPServerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/dhcp_server/DHCPServerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/dhcp_server/DHCPServerFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/dhcp_server/DHCPServerFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureBase.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureBase.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/NonlinearityEEPROMSlotFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/NonlinearityEEPROMSlotFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeatureBase.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeatureBase.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_MayaPro.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_MayaPro.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_NIRQuest.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_NIRQuest.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SerialNumberEEPROMSlotFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/SerialNumberEEPROMSlotFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/StrayLightEEPROMSlotFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/StrayLightEEPROMSlotFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature_QE65000.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature_QE65000.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureBase.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureBase.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FlameXFastBufferFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/fast_buffer/FlameXFastBufferFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/fpga_register/FPGARegisterFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/fpga_register/FPGARegisterFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/fpga_register/FPGARegisterFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/fpga_register/FPGARegisterFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/gpio/gpioFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/gpio/gpioFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/gpio/gpioFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/gpio/gpioFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/i2c_master/i2cMasterFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/i2c_master/i2cMasterFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/i2c_master/i2cMasterFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/i2c_master/i2cMasterFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/introspection/IntrospectionFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/introspection/IntrospectionFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/introspection/IntrospectionFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/introspection/IntrospectionFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/ipv4/IPv4Feature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/ipv4/IPv4Feature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/ipv4/IPv4FeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/ipv4/IPv4FeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/irradcal/IrradCalFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/irradcal/IrradCalFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/irradcal/IrradCalFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/irradcal/IrradCalFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureBase.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureBase.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureImpl.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureImpl.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/LightSourceFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/StrobeLampFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/StrobeLampFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/StrobeLampFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/StrobeLampFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/VentanaLightSourceFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/light_source/VentanaLightSourceFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/multicast/MulticastFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/multicast/MulticastFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/multicast/MulticastFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/multicast/MulticastFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/optical_bench/OpticalBenchFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/optical_bench/OpticalBenchFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/optical_bench/OpticalBenchFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/optical_bench/OpticalBenchFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/pixel_binning/PixelBinningFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/pixel_binning/PixelBinningFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/pixel_binning/STSPixelBinningFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/pixel_binning/STSPixelBinningFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/revision/RevisionFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/revision/RevisionFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/revision/RevisionFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/revision/RevisionFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/serial_number/SerialNumberFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/serial_number/SerialNumberFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/serial_number/SerialNumberFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/serial_number/SerialNumberFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/shutter/ShutterFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/shutter/ShutterFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/shutter/ShutterFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/shutter/ShutterFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ApexSpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ApexSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/FlameNIRSpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/FlameNIRSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/FlameXSpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/FlameXSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/GainAdjustedSpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/GainAdjustedSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR2000PlusSpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR2000PlusSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR2000SpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR2000SpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR4000SpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/HR4000SpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/JazSpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/JazSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/Maya2000ProSpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/Maya2000ProSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/Maya2000SpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/Maya2000SpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/MayaLSLSpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/MayaLSLSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuest256SpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuest256SpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuest512SpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuest512SpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuestSpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/NIRQuestSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureBase.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureBase.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureImpl.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureImpl.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/QE65000SpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/QE65000SpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/QEProSpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/QEProSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/STSSpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/STSSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/SparkSpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/SparkSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/SpectrometerTriggerMode.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/SpectrometerTriggerMode.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB2000PlusSpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB2000PlusSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB2000SpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB2000SpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB4000SpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/USB4000SpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/VentanaSpectrometerFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrometer/VentanaSpectrometerFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/temperature/TemperatureFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/temperature/TemperatureFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/temperature/TemperatureFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/temperature/TemperatureFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/QEProThermoElectricFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/QEProThermoElectricFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureBase.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureBase.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricQEFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/ThermoElectricQEFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/VentanaThermoElectricFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/thermoelectric/VentanaThermoElectricFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/wavecal/WaveCalFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/wavecal/WaveCalFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/wavecal/WaveCalFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/wavecal/WaveCalFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeature.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeature.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeatureInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeatureInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/AcquisitionDelayProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/AcquisitionDelayProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ContinuousStrobeProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ContinuousStrobeProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/DHCPServerProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/DHCPServerProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/DataBufferProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/DataBufferProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/EEPROMProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/EEPROMProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/EthernetConfigurationProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/EthernetConfigurationProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/FPGARegisterProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/FPGARegisterProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/FastBufferProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/FastBufferProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/GPIOProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/GPIOProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/I2CMasterProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/I2CMasterProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IPv4ProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IPv4ProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IntrospectionProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IntrospectionProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IrradCalProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/IrradCalProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/LightSourceProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/LightSourceProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/MulticastProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/MulticastProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/NetworkConfigurationProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/NetworkConfigurationProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/NonlinearityCoeffsProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/NonlinearityCoeffsProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/OpticalBenchProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/OpticalBenchProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/PixelBinningProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/PixelBinningProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ProgrammableSaturationProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ProgrammableSaturationProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/RevisionProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/RevisionProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SerialNumberProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SerialNumberProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ShutterProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ShutterProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SpectrometerProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SpectrometerProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SpectrumProcessingProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/SpectrumProcessingProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/StrayLightCoeffsProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/StrayLightCoeffsProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/StrobeLampProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/StrobeLampProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/TemperatureProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/TemperatureProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ThermoElectricProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/ThermoElectricProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/WaveCalProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/WaveCalProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/WifiConfigurationProtocolInterface.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/interfaces/WifiConfigurationProtocolInterface.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/constants/OBPMessageTypes.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/constants/OBPMessageTypes.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPAddIPv4AddressExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPAddIPv4AddressExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPCommand.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPCommand.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobeEnableExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobeEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobePeriodExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobePeriodExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferClearExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferClearExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferRemoveOldestExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferRemoveOldestExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDeleteIPv4AddressExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPDeleteIPv4AddressExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetActivePixelRangesExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetActivePixelRangesExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetAllTemperaturesExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetAllTemperaturesExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetBoxcarWidthExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetBoxcarWidthExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetConsecutiveSampleCountExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetConsecutiveSampleCountExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerAddressExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerAddressExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerEnableExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCapacityExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCapacityExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferElementCountExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferElementCountExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferMaximumCapacityExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferMaximumCapacityExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDefaultPixelBinningExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDefaultPixelBinningExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetElectricDarkPixelRangesExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetElectricDarkPixelRangesExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationGbEEnableExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationGbEEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationMACAddressExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationMACAddressExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFastBufferingEnableExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFastBufferingEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFirmwareRevisionExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFirmwareRevisionExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionAvailableModesExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionAvailableModesExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionCurrentModeExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionCurrentModeExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionNumberOfPinsExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionNumberOfPinsExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionOutputVectorExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionOutputVectorExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionValueExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionValueExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIONumberOfPinsExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIONumberOfPinsExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOOutputEnableVectorExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOOutputEnableVectorExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOValueVectorExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOValueVectorExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetHardwareRevisionExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetHardwareRevisionExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetI2CMasterNumberOfBusesExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetI2CMasterNumberOfBusesExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4AddressExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4AddressExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DHCPEnableStateExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DHCPEnableStateExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DefaultGatewayExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DefaultGatewayExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4NumberOfAddressesExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4NumberOfAddressesExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCalExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCalExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCollectionAreaExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCollectionAreaExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMaxPixelBinningExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMaxPixelBinningExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMulticastEnableExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMulticastEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceConnectionTypeExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceConnectionTypeExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceEnableStateExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceEnableStateExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffsCountExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffsCountExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfNetworkInterfacesExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfNetworkInterfacesExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfPixelsExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfPixelsExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchCoatingExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchCoatingExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFiberDiameterMicronsExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFiberDiameterMicronsExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFilterExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFilterExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchGratingExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchGratingExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchIDExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchIDExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSerialNumberExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSerialNumberExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSlitWidthMicronsExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSlitWidthMicronsExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalDarkPixelRangesExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalDarkPixelRangesExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetPixelBinningExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetPixelBinningExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSaturationExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSaturationExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetScansToAverageExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetScansToAverageExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberMaximumLengthExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberMaximumLengthExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffsCountExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffsCountExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureCountExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureCountExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetThermoElectricTemperatureExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetThermoElectricTemperatureExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWaveCalExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWaveCalExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationModeExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationModeExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSSIDExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSSIDExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSecurityExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSecurityExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPIntegrationTimeExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPIntegrationTimeExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLampEnableCommand.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLampEnableCommand.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnableCommand.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnableCommand.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnabledQuery.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnabledQuery.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityCommand.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityCommand.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityQuery.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityQuery.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPMessage.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPMessage.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPQuery.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPQuery.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadI2CMasterBusExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadI2CMasterBusExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadNumberOfRawSpectraWithMetadataExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadNumberOfRawSpectraWithMetadataExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrum32AndMetadataExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrum32AndMetadataExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrumExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrum32AndMetadataExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrum32AndMetadataExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumWithGainExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumWithGainExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestBufferedSpectrum32AndMetadataExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestBufferedSpectrum32AndMetadataExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestNumberOfBufferedSpectraWithMetadataExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestNumberOfBufferedSpectraWithMetadataExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestRawSpectrumExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestRawSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestSpectrumExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRunNetworkInterfaceSelfTestExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPRunNetworkInterfaceSelfTestExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSaveNetworkInterfaceConnectionSettingsExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSaveNetworkInterfaceConnectionSettingsExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetAcquisitionDelayExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetAcquisitionDelayExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetBoxcarWidthExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetBoxcarWidthExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetConsecutiveSampleCountExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetConsecutiveSampleCountExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerAddressExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerAddressExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerEnableExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDataBufferCapacityExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDataBufferCapacityExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDefaultPixelBinningExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDefaultPixelBinningExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationGbEEnableExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationGbEEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationMACAddressExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationMACAddressExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetFastBufferingEnableExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetFastBufferingEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionModeExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionModeExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionOutputVectorExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionOutputVectorExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionValueExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionValueExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionVectorExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionVectorExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOOutputEnableVectorExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOOutputEnableVectorExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOValueVectorExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOValueVectorExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DHCPEnableStateExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DHCPEnableStateExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DefaultGatewayExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DefaultGatewayExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCalExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCalExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCollectionAreaExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCollectionAreaExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetMulticastEnableExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetMulticastEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetNetworkInterfaceEnableStateExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetNetworkInterfaceEnableStateExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetPixelBinningExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetPixelBinningExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetScansToAverageExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetScansToAverageExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricEnableExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricSetpointExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricSetpointExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationModeExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationModeExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationPassPhraseExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationPassPhraseExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSSIDExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSSIDExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSecurityExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSecurityExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPShutterExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPShutterExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPTransaction.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPTransaction.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPTriggerModeExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPTriggerModeExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPWriteI2CMasterBusExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/exchanges/OBPWriteI2CMasterBusExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/hints/OBPControlHint.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/hints/OBPControlHint.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/hints/OBPSpectrumHint.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/hints/OBPSpectrumHint.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPAcquisitionDelayProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPAcquisitionDelayProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPContinuousStrobeProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPContinuousStrobeProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPDHCPServerProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPDHCPServerProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPDataBufferProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPDataBufferProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPEthernetConfigurationProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPEthernetConfigurationProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPFastBufferProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPFastBufferProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPGPIOProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPGPIOProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPI2CMasterProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPI2CMasterProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIPv4Protocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIPv4Protocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIntrospectionProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIntrospectionProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIrradCalProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPIrradCalProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol_Ventana.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol_Ventana.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPMulticastProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPMulticastProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPNetworkConfigurationProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPNetworkConfigurationProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPNonlinearityCoeffsProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPNonlinearityCoeffsProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPOpticalBenchProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPOpticalBenchProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPPixelBinningProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPPixelBinningProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPProgrammableSaturationProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPProgrammableSaturationProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPRevisionProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPRevisionProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSerialNumberProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSerialNumberProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPShutterProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPShutterProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSpectrometerProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSpectrometerProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSpectrumProcessingProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPSpectrumProcessingProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPStrayLightCoeffsProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPStrayLightCoeffsProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPStrobeLampProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPStrobeLampProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPTemperatureProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPTemperatureProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPThermoElectricProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPThermoElectricProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPWaveCalProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPWaveCalProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPWifiConfigurationProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OBPWifiConfigurationProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OceanBinaryProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/obp/impls/OceanBinaryProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/FPGARegisterCodes.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/FPGARegisterCodes.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/OpCodes.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/OpCodes.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/QETECConstants.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/constants/QETECConstants.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterReadExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterReadExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterWriteExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterWriteExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGASpectrumExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FPGASpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FlameNIRSpectrumExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/FlameNIRSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/HRFPGASpectrumExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/HRFPGASpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/IntegrationTimeExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/IntegrationTimeExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/JazSpectrumExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/JazSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/MayaProSpectrumExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/MayaProSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/NIRQuestSpectrumExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/NIRQuestSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOI2KSpectrumExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOI2KSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIIrradCalExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIIrradCalExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIReadIrradCalExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIReadIrradCalExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIWriteIrradCalExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/OOIWriteIrradCalExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/QESpectrumExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/QESpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadEEPROMSlotExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadEEPROMSlotExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadSpectrumExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECQETemperatureExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECQETemperatureExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECTemperatureExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECTemperatureExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/RequestSpectrumExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/RequestSpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/StrobeEnableExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/StrobeEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TECEnableExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TECEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TECQEEnableExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TECQEEnableExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TriggerModeExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/TriggerModeExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/USBFPGASpectrumExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/USBFPGASpectrumExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteEEPROMSlotExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteEEPROMSlotExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECQESetPointExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECQESetPointExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECSetPointExchange.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECSetPointExchange.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/hints/ControlHint.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/hints/ControlHint.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/hints/SpectrumHint.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/hints/SpectrumHint.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/FPGARegisterProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/FPGARegisterProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIEEPROMProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIEEPROMProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIIrradCalProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIIrradCalProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOISpectrometerProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOISpectrometerProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIStrobeLampProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOIStrobeLampProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOITECProtocol.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/protocols/ooi/impls/OOITECProtocol.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/include/vendors/OceanOptics/utils/Polynomial.h` & `seabreeze-2.8.0/src/libseabreeze/include/vendors/OceanOptics/utils/Polynomial.h`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/DeviceFactory.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/DeviceFactory.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/AcquisitionDelayFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/AcquisitionDelayFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/ContinuousStrobeFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/ContinuousStrobeFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/DHCPServerFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/DHCPServerFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/DataBufferFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/DataBufferFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/DeviceAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/DeviceAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/EEPROMFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/EEPROMFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/EthernetConfigurationFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/EthernetConfigurationFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/FastBufferFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/FastBufferFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/FeatureFamilies.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/FeatureFamilies.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/I2CMasterFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/I2CMasterFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/IPv4FeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/IPv4FeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/IntrospectionFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/IntrospectionFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/IrradCalFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/IrradCalFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/LightSourceFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/LightSourceFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/MulticastFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/MulticastFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/NetworkConfigurationFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/NetworkConfigurationFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/NonlinearityCoeffsFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/NonlinearityCoeffsFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/OpticalBenchFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/OpticalBenchFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/PixelBinningFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/PixelBinningFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/ProtocolFamilies.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/ProtocolFamilies.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/RawUSBBusAccessFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/RawUSBBusAccessFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/RevisionFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/RevisionFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/SeaBreezeAPI.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/SeaBreezeAPI.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/SeaBreezeAPI_Impl.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/SeaBreezeAPI_Impl.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/SerialNumberFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/SerialNumberFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/ShutterFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/ShutterFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/SpectrometerFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/SpectrometerFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/SpectrumProcessingFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/SpectrumProcessingFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/StrayLightCoeffsFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/StrayLightCoeffsFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/StrobeLampFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/StrobeLampFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/TemperatureFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/TemperatureFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/ThermoElectricCoolerFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/ThermoElectricCoolerFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/WifiConfigurationFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/WifiConfigurationFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/api/seabreezeapi/gpioFeatureAdapter.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/api/seabreezeapi/gpioFeatureAdapter.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/ByteVector.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/ByteVector.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/Data.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/Data.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/DoubleVector.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/DoubleVector.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/FloatVector.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/FloatVector.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/Log.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/Log.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/U32Vector.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/U32Vector.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/UShortVector.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/UShortVector.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/UnitDescriptor.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/UnitDescriptor.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/buses/Bus.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/buses/Bus.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/buses/BusFamilies.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/buses/BusFamilies.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/buses/BusFamily.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/buses/BusFamily.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/buses/DeviceLocationProberInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/buses/DeviceLocationProberInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/buses/TransferHelper.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/buses/TransferHelper.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/buses/network/IPv4NetworkProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/buses/network/IPv4NetworkProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/buses/network/IPv4SocketDeviceLocator.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/buses/network/IPv4SocketDeviceLocator.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/buses/network/TCPIPv4SocketBus.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/buses/network/TCPIPv4SocketBus.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/buses/network/TCPIPv4SocketTransferHelper.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/buses/network/TCPIPv4SocketTransferHelper.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/buses/rs232/RS232DeviceLocator.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/buses/rs232/RS232DeviceLocator.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/buses/rs232/RS232Interface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/buses/rs232/RS232Interface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/buses/rs232/RS232TransferHelper.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/buses/rs232/RS232TransferHelper.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/buses/usb/USBDeviceLocator.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/buses/usb/USBDeviceLocator.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/buses/usb/USBInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/buses/usb/USBInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/buses/usb/USBTransferHelper.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/buses/usb/USBTransferHelper.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/devices/Device.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/devices/Device.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/BusConnectException.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/BusConnectException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/BusException.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/BusException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/BusTransferException.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/BusTransferException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/FeatureControlException.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/FeatureControlException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/FeatureException.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/FeatureException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/FeatureProtocolNotFoundException.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/FeatureProtocolNotFoundException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/IllegalArgumentException.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/IllegalArgumentException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/NumberFormatException.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/NumberFormatException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/ProtocolBusMismatchException.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/ProtocolBusMismatchException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/ProtocolException.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/ProtocolException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/ProtocolFormatException.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/ProtocolFormatException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/exceptions/ProtocolTransactionException.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/exceptions/ProtocolTransactionException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/features/FeatureFamily.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/features/FeatureFamily.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/features/FeatureImpl.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/features/FeatureImpl.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/protocols/Exchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/protocols/Exchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/protocols/Protocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/protocols/Protocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/protocols/ProtocolFamily.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/protocols/ProtocolFamily.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/protocols/ProtocolHelper.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/protocols/ProtocolHelper.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/protocols/ProtocolHint.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/protocols/ProtocolHint.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/protocols/Transaction.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/protocols/Transaction.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/common/protocols/Transfer.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/common/protocols/Transfer.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/native/network/Inet4Address.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/native/network/Inet4Address.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/native/network/SocketException.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/native/network/SocketException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/native/network/SocketTimeoutException.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/native/network/SocketTimeoutException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/native/network/UnknownHostException.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/native/network/UnknownHostException.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/native/network/posix/NativeSocketPOSIX.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/native/network/posix/NativeSocketPOSIX.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/native/network/windows/NativeSocketWindows.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/native/network/windows/NativeSocketWindows.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/native/rs232/RS232.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/native/rs232/RS232.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/native/rs232/posix/NativeRS232POSIX.c` & `seabreeze-2.8.0/src/libseabreeze/src/native/rs232/posix/NativeRS232POSIX.c`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/native/rs232/windows/NativeRS232Windows.c` & `seabreeze-2.8.0/src/libseabreeze/src/native/rs232/windows/NativeRS232Windows.c`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/native/system/System.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/native/system/System.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/native/system/posix/NativeSystemPOSIX.c` & `seabreeze-2.8.0/src/libseabreeze/src/native/system/posix/NativeSystemPOSIX.c`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/native/system/windows/NativeSystemWindows.c` & `seabreeze-2.8.0/src/libseabreeze/src/native/system/windows/NativeSystemWindows.c`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/native/usb/USB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/native/usb/USB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/native/usb/USBDiscovery.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/native/usb/USBDiscovery.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/native/usb/linux/NativeUSBLinux.c` & `seabreeze-2.8.0/src/libseabreeze/src/native/usb/linux/NativeUSBLinux.c`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/native/usb/osx/NativeUSBMacOSX.c` & `seabreeze-2.8.0/src/libseabreeze/src/native/usb/osx/NativeUSBMacOSX.c`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/native/usb/winusb/NativeUSBWinUSB.c` & `seabreeze-2.8.0/src/libseabreeze/src/native/usb/winusb/NativeUSBWinUSB.c`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/network/FlameXTCPIPv4.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/network/FlameXTCPIPv4.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/network/JazTCPIPv4.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/network/JazTCPIPv4.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/rs232/OOIRS232Interface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/rs232/OOIRS232Interface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/ApexUSB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/ApexUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameNIRUSB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameNIRUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameXUSB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameXUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameXUSBTransferHelper.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/FlameXUSBTransferHelper.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR2000PlusUSB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR2000PlusUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR2000USB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR2000USB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR4000USB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/HR4000USB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/JazUSB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/JazUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/Maya2000ProUSB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/Maya2000ProUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/Maya2000USB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/Maya2000USB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/MayaLSLUSB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/MayaLSLUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/NIRQuest256USB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/NIRQuest256USB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/NIRQuest512USB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/NIRQuest512USB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSB4KSpectrumTransferHelper.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSB4KSpectrumTransferHelper.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBControlTransferHelper.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBControlTransferHelper.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBEndpointMaps.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBEndpointMaps.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBSpectrumTransferHelper.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBSpectrumTransferHelper.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBTrivialTransferHelper.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/OOIUSBTrivialTransferHelper.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/QE65000USB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/QE65000USB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/QEProUSB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/QEProUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/STSUSB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/STSUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/SparkUSB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/SparkUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/TorusUSB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/TorusUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB2000PlusUSB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB2000PlusUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB2000USB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB2000USB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB4000USB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/USB4000USB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/VentanaUSB.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/buses/usb/VentanaUSB.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/Apex.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/Apex.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/FlameNIR.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/FlameNIR.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/FlameX.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/FlameX.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR2000.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR2000.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR2000Plus.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR2000Plus.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR4000.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/HR4000.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/Jaz.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/Jaz.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/Maya2000.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/Maya2000.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/Maya2000Pro.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/Maya2000Pro.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/MayaLSL.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/MayaLSL.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/NIRQuest256.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/NIRQuest256.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/NIRQuest512.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/NIRQuest512.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/QE65000.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/QE65000.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/QEPro.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/QEPro.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/STS.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/STS.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/Spark.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/Spark.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/Torus.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/Torus.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB2000.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB2000.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB2000Plus.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB2000Plus.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB4000.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/USB4000.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/devices/Ventana.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/devices/Ventana.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature_FPGA.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/AcquisitionDelayFeature_FPGA.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/STSAcquisitionDelayFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/acquisition_delay/STSAcquisitionDelayFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature_FPGA.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/continuous_strobe/ContinuousStrobeFeature_FPGA.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/DataBufferFeatureBase.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/DataBufferFeatureBase.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/FlameXDataBufferFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/FlameXDataBufferFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/QEProDataBufferFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/data_buffer/QEProDataBufferFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/dhcp_server/DHCPServerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/dhcp_server/DHCPServerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureBase.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/EEPROMSlotFeatureBase.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/NonlinearityEEPROMSlotFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/NonlinearityEEPROMSlotFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeatureBase.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeatureBase.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_MayaPro.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_MayaPro.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_NIRQuest.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SaturationEEPROMSlotFeature_NIRQuest.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SerialNumberEEPROMSlotFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/SerialNumberEEPROMSlotFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/StrayLightEEPROMSlotFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/StrayLightEEPROMSlotFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature_QE65000.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/eeprom_slots/WavelengthEEPROMSlotFeature_QE65000.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/ethernet_configuration/EthernetConfigurationFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureBase.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/fast_buffer/FastBufferFeatureBase.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/fast_buffer/FlameXFastBufferFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/fast_buffer/FlameXFastBufferFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/fpga_register/FPGARegisterFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/fpga_register/FPGARegisterFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/gpio/gpioFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/gpio/gpioFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/i2c_master/i2cFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/i2c_master/i2cFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/introspection/IntrospectionFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/introspection/IntrospectionFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/ipv4/IPv4Feature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/ipv4/IPv4Feature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/irradcal/IrradCalFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/irradcal/IrradCalFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/LightSourceFeatureBase.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/LightSourceFeatureBase.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/LightSourceFeatureImpl.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/LightSourceFeatureImpl.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/StrobeLampFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/StrobeLampFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/VentanaLightSourceFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/light_source/VentanaLightSourceFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/multicast/MulticastFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/multicast/MulticastFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/network_configuration/NetworkConfigurationFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/nonlinearity/NonlinearityCoeffsFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/optical_bench/OpticalBenchFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/optical_bench/OpticalBenchFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/pixel_binning/PixelBinningFeatureInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/pixel_binning/PixelBinningFeatureInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/pixel_binning/STSPixelBinningFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/pixel_binning/STSPixelBinningFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/raw_bus_access/RawUSBBusAccessFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/revision/RevisionFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/revision/RevisionFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/serial_number/SerialNumberFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/serial_number/SerialNumberFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/shutter/ShutterFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/shutter/ShutterFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ApexSpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ApexSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/FlameNIRSpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/FlameNIRSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/FlameXSpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/FlameXSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/GainAdjustedSpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/GainAdjustedSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR2000PlusSpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR2000PlusSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR2000SpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR2000SpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR4000SpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/HR4000SpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/JazSpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/JazSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/Maya2000ProSpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/Maya2000ProSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/Maya2000SpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/Maya2000SpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/MayaLSLSpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/MayaLSLSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuest256SpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuest256SpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuest512SpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuest512SpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuestSpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/NIRQuestSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/OOISpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureBase.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureBase.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureImpl.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/ProgrammableSaturationFeatureImpl.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/QE65000SpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/QE65000SpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/QEProSpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/QEProSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/STSSpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/STSSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/SparkSpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/SparkSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/SpectrometerTriggerMode.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/SpectrometerTriggerMode.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB2000PlusSpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB2000PlusSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB2000SpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB2000SpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB4000SpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/USB4000SpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/VentanaSpectrometerFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrometer/VentanaSpectrometerFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/spectrum_processing/SpectrumProcessingFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/stray_light/StrayLightCoeffsFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/temperature/TemperatureFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/temperature/TemperatureFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/QEProThermoElectricFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/QEProThermoElectricFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureBase.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/ThermoElectricFeatureBase.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/ThermoElectricQEFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/ThermoElectricQEFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/VentanaThermoElectricFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/thermoelectric/VentanaThermoElectricFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/wavecal/WaveCalFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/wavecal/WaveCalFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeature.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/features/wifi_configuration/WifiConfigurationFeature.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/AcquisitionDelayProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/AcquisitionDelayProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ContinuousStrobeProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ContinuousStrobeProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/DHCPServerProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/DHCPServerProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/DataBufferProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/DataBufferProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/EEPROMProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/EEPROMProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/EthernetConfigurationProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/EthernetConfigurationProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/FPGARegisterProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/FPGARegisterProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/FastBufferProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/FastBufferProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/GPIOProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/GPIOProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/I2CMasterProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/I2CMasterProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IPv4ProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IPv4ProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IntrospectionProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IntrospectionProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IrradCalProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/IrradCalProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/LightSourceProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/LightSourceProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/MulticastProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/MulticastProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/NetworkConfigurationProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/NetworkConfigurationProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/NonlinearityCoeffsProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/NonlinearityCoeffsProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/OpticalBenchProtocolInteface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/OpticalBenchProtocolInteface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/PixelBinningProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/PixelBinningProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ProgrammableSaturationProtocolInteface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ProgrammableSaturationProtocolInteface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/RevisionProtocolInteface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/RevisionProtocolInteface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SerialNumberProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SerialNumberProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ShutterProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ShutterProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SpectrometerProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SpectrometerProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SpectrumProcessingProtocolInteface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/SpectrumProcessingProtocolInteface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/StrayLightCoeffsProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/StrayLightCoeffsProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/StrobeLampProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/StrobeLampProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/TemperatureProtocolInteface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/TemperatureProtocolInteface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ThermoElectricProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/ThermoElectricProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/WaveCalProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/WaveCalProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/WifiConfigurationProtocolInterface.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/interfaces/WifiConfigurationProtocolInterface.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPAddIPv4AddressExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPAddIPv4AddressExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPCommand.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPCommand.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobeEnableExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobeEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobePeriodExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPContinuousStrobePeriodExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferClearExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferClearExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferRemoveOldestExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDataBufferRemoveOldestExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDeleteIPv4AddressExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPDeleteIPv4AddressExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetActivePixelRangesExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetActivePixelRangesExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetAllTemperaturesExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetAllTemperaturesExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetBoxcarWidthExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetBoxcarWidthExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetConsecutiveSampleCountExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetConsecutiveSampleCountExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerAddressExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerAddressExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerEnableExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDHCPServerEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCapacityExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCapacityExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCountExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferCountExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferMaximumCapacityExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDataBufferMaximumCapacityExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDefaultPixelBinningExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetDefaultPixelBinningExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetElectricDarkPixelRangesExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetElectricDarkPixelRangesExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationGbEEnableExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationGbEEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationMACAddressExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetEthernetConfigurationMACAddressExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFastBufferingEnableExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFastBufferingEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFirmwareRevisionExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetFirmwareRevisionExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionAvailableModesExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionAvailableModesExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionCurrentModeExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionCurrentModeExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionNumberOfPinsExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionNumberOfPinsExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionOutputVectorExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionOutputVectorExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionValueExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOExtensionValueExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIONumberOfPinsExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIONumberOfPinsExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOOutputEnableVectorExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOOutputEnableVectorExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOValueVectorExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetGPIOValueVectorExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetHardwareRevisionExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetHardwareRevisionExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetI2CMasterNumberOfBusesExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetI2CMasterNumberOfBusesExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4AddressExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4AddressExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DHCPEnableStateExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DHCPEnableStateExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DefaultGatewayExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4DefaultGatewayExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4NumberOfAddressesExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIPv4NumberOfAddressesExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCalExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCalExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCollectionAreaExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetIrradCollectionAreaExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMaxPixelBinningExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMaxPixelBinningExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMulticastEnableExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetMulticastEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceConnectionTypeExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceConnectionTypeExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceEnableStateExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNetworkInterfaceEnableStateExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffsCountExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNonlinearityCoeffsCountExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfNetworkInterfacesExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfNetworkInterfacesExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfPixelsExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetNumberOfPixelsExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchCoatingExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchCoatingExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFiberDiameterMicronsExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFiberDiameterMicronsExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFilterExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchFilterExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchGratingExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchGratingExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchIDExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchIDExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSerialNumberExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSerialNumberExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSlitWidthMicronsExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalBenchSlitWidthMicronsExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalDarkPixelRangesExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetOpticalDarkPixelRangesExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetPixelBinningExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetPixelBinningExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSaturationExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSaturationExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetScansToAverageExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetScansToAverageExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberMaximumLengthExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetSerialNumberMaximumLengthExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffsCountExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetStrayLightCoeffsCountExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureCountExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureCountExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetTemperatureExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetThermoElectricTemperatureExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetThermoElectricTemperatureExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWaveCalExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWaveCalExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationModeExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationModeExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSSIDExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSSIDExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSecurityExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPGetWifiConfigurationSecurityExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPIntegrationTimeExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPIntegrationTimeExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLampEnableCommand.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLampEnableCommand.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnableCommand.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnableCommand.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnabledQuery.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceEnabledQuery.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityCommand.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityCommand.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityQuery.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPLightSourceIntensityQuery.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPMessage.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPMessage.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPQuery.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPQuery.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadI2CMasterBusExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadI2CMasterBusExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadNumberOfRawSpectraWithMetadataExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadNumberOfRawSpectraWithMetadataExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrum32AndMetadataExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrum32AndMetadataExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrumExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadRawSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrum32AndMetadataExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrum32AndMetadataExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumWithGainExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPReadSpectrumWithGainExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestBufferedSpectrum32AndMetadata.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestBufferedSpectrum32AndMetadata.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestNumberOfBufferedSpectraWithMetadata.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestNumberOfBufferedSpectraWithMetadata.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestRawSpectrumExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestRawSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestSpectrumExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRequestSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRunNetworkInterfaceSelfTestExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPRunNetworkInterfaceSelfTestExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSaveNetworkInterfaceConnectionSettingsExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSaveNetworkInterfaceConnectionSettingsExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetAcquisitionDelayExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetAcquisitionDelayExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetBoxcarWidthExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetBoxcarWidthExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetConsecutiveSampleCountExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetConsecutiveSampleCountExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerAddressExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerAddressExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerEnableExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDHCPServerEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDataBufferCapacityExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDataBufferCapacityExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDefaultPixelBinningFactorExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetDefaultPixelBinningFactorExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationGbEEnableExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationGbEEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationMACAddressExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetEthernetConfigurationMACAddressExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetFastBufferingEnableExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetFastBufferingEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionModeExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionModeExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionOutputVectorExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionOutputVectorExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionValueExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOExtensionValueExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOOutputEnableVectorExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOOutputEnableVectorExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOValueVectorExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetGPIOValueVectorExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DHCPEnableStateExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DHCPEnableStateExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DefaultGatewayExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIPv4DefaultGatewayExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCalExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCalExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCollectionAreaExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetIrradCollectionAreaExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetMulticastEnableExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetMulticastEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetNetworkInterfaceEnableStateExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetNetworkInterfaceEnableStateExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetPixelBinningExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetPixelBinningExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetScansToAverageExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetScansToAverageExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricEnableExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricSetpointExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetThermoElectricSetpointExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationModeExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationModeExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationPassPhraseExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationPassPhraseExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSSIDExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSSIDExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSecurityExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPSetWifiConfigurationSecurityExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPShutterExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPShutterExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPTransaction.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPTransaction.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPTriggerModeExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPTriggerModeExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPWriteI2CMasterBusExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/exchanges/OBPWriteI2CMasterBusExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/hints/OBPControlHint.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/hints/OBPControlHint.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/hints/OBPSpectrumHint.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/hints/OBPSpectrumHint.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPAcquisitionDelayProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPAcquisitionDelayProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPContinuousStrobeProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPContinuousStrobeProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPDHCPServerProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPDHCPServerProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPDataBufferProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPDataBufferProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPEthernetConfigurationProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPEthernetConfigurationProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPFastBufferProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPFastBufferProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPGPIOProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPGPIOProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPI2CMasterProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPI2CMasterProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIPv4Protocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIPv4Protocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIntrospectionProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIntrospectionProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIrradCalProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPIrradCalProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol_Ventana.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPLightSourceProtocol_Ventana.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPMulticastProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPMulticastProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPNetworkConfigurationProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPNetworkConfigurationProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPNonlinearityCoeffsProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPNonlinearityCoeffsProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPOpticalBenchProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPOpticalBenchProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPPixelBinningProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPPixelBinningProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPProgrammableSaturationProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPProgrammableSaturationProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPRevisionProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPRevisionProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSerialNumberProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSerialNumberProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPShutterProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPShutterProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSpectrometerProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSpectrometerProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSpectrumProcessingProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPSpectrumProcessingProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPStrayLightCoeffsProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPStrayLightCoeffsProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPStrobeLampProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPStrobeLampProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPTemperatureProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPTemperatureProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPThermoElectricProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPThermoElectricProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPWaveCalProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPWaveCalProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPWifiConfigurationProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OBPWifiConfigurationProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OceanBinaryProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/obp/impls/OceanBinaryProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/constants/FPGARegisterCodes.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/constants/FPGARegisterCodes.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/constants/OpCodes.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/constants/OpCodes.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterReadExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterReadExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterWriteExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGARegisterWriteExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGASpectrumExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FPGASpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FlameNIRSpectrumExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/FlameNIRSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/HRFPGASpectrumExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/HRFPGASpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/IntegrationTimeExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/IntegrationTimeExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/JazSpectrumExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/JazSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/MayaProSpectrumExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/MayaProSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/NIRQuestSpectrumExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/NIRQuestSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOI2KSpectrumExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOI2KSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIIrradCalExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIIrradCalExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIReadIrradCalExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIReadIrradCalExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIWriteIrradCalExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/OOIWriteIrradCalExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/QESpectrumExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/QESpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadEEPROMSlotExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadEEPROMSlotExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadSpectrumExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECQETemperatureExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECQETemperatureExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECTemperatureExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/ReadTECTemperatureExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/RequestSpectrumExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/RequestSpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/StrobeEnableExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/StrobeEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TECEnableExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TECEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TECQEEnableExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TECQEEnableExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TriggerModeExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/TriggerModeExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/USBFPGASpectrumExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/USBFPGASpectrumExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteEEPROMSlotExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteEEPROMSlotExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECQESetPointExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECQESetPointExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECSetPointExchange.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/exchanges/WriteTECSetPointExchange.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/hints/ControlHint.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/hints/ControlHint.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/hints/SpectrumHint.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/hints/SpectrumHint.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/FPGARegisterProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/FPGARegisterProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIEEPROMProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIEEPROMProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIIrradCalProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIIrradCalProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOISpectrometerProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOISpectrometerProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIStrobeLampProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOIStrobeLampProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOITECProtocol.cpp` & `seabreeze-2.8.0/src/libseabreeze/src/vendors/OceanOptics/protocols/ooi/impls/OOITECProtocol.cpp`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/__init__.py` & `seabreeze-2.8.0/src/seabreeze/__init__.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/_cli.py` & `seabreeze-2.8.0/src/seabreeze/_cli.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/backends.py` & `seabreeze-2.8.0/src/seabreeze/backends.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/cseabreeze/__init__.py` & `seabreeze-2.8.0/src/seabreeze/cseabreeze/__init__.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/cseabreeze/c_seabreeze.pxd` & `seabreeze-2.8.0/src/seabreeze/cseabreeze/c_seabreeze.pxd`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/cseabreeze/c_seabreeze_wrapper.pyx` & `seabreeze-2.8.0/src/seabreeze/cseabreeze/c_seabreeze_wrapper.pyx`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/os_setup.py` & `seabreeze-2.8.0/src/seabreeze/os_setup.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/__init__.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/__init__.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/api.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/api.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/config.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/config.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/devices.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,15 @@
         """dark pixel indices
 
         Parameters
         ----------
         indices : iterable
             index of electric dark pixel
         """
-        return super().__new__(DarkPixelIndices, sorted(set(indices)))  # type: ignore
+        return super().__new__(DarkPixelIndices, sorted(set(indices)))
 
     @classmethod
     def from_ranges(cls, *ranges: tuple[int, int]) -> DarkPixelIndices:
         """return dark pixes indices from ranges
 
         Parameters
         ----------
@@ -1272,14 +1272,62 @@
     spectrum_max_value = 65535
     trigger_modes = TriggerMode.supported("OBP_NORMAL")
 
     # features
     feature_classes = (sbf.spectrometer.SeaBreezeSpectrometerFeatureSR6,)
 
 
+class HR2(SeaBreezeDevice):
+    model_name = "HR2"
+
+    # communication config
+    transport = (USBTransport,)
+    usb_vendor_id = 0x0999
+    usb_product_id = 0x1003
+    usb_endpoint_map = EndPointMap(ep_out=0x01, highspeed_in=0x81)
+    usb_protocol = OBP2Protocol
+
+    # spectrometer config
+    dark_pixel_indices = DarkPixelIndices.from_ranges()
+    integration_time_min = 1  # 1 us
+    integration_time_max = 2000000  # 2 s
+    integration_time_base = 1
+    spectrum_num_pixel = 2110
+    spectrum_raw_length = (2110 * 2) + 32  # XXX: Metadata
+    spectrum_max_value = 65535
+    trigger_modes = TriggerMode.supported("OBP_NORMAL")
+
+    # features
+    feature_classes = (sbf.spectrometer.SeaBreezeSpectrometerFeatureHR2,)
+
+
+class HR4(SeaBreezeDevice):
+    model_name = "HR4"
+
+    # communication config
+    transport = (USBTransport,)
+    usb_vendor_id = 0x0999
+    usb_product_id = 0x1004
+    usb_endpoint_map = EndPointMap(ep_out=0x01, highspeed_in=0x81)
+    usb_protocol = OBP2Protocol
+
+    # spectrometer config
+    dark_pixel_indices = DarkPixelIndices.from_ranges()
+    integration_time_min = 3800  # 3.8ms
+    integration_time_max = 10000000  # 10s
+    integration_time_base = 1
+    spectrum_num_pixel = 3648
+    spectrum_raw_length = (3648 * 2) + 32  # XXX: Metadata
+    spectrum_max_value = 65535
+    trigger_modes = TriggerMode.supported("OBP_NORMAL")
+
+    # features
+    feature_classes = (sbf.spectrometer.SeaBreezeSpectrometerFeatureHR4,)
+
+
 class ST(SeaBreezeDevice):
     model_name = "ST"
 
     # communication config
     transport = (USBTransport,)
     usb_vendor_id = 0x0999
     usb_product_id = 0x1000
```

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/__init__.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/__init__.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/_base.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/_base.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/acquisitiondelay.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/acquisitiondelay.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/continuousstrobe.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/continuousstrobe.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/databuffer.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/databuffer.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/dhcpserver.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/dhcpserver.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/eeprom.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/eeprom.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/ethernetconfiguration.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/ethernetconfiguration.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/fastbuffer.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/fastbuffer.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/fpga.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/fpga.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/gpio.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/gpio.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/i2cmaster.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/i2cmaster.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/introspection.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/introspection.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/ipv4.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/ipv4.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/irradcal.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/irradcal.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/lightsource.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/lightsource.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/multicast.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/multicast.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/networkconfiguration.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/networkconfiguration.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/nonlinearity.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/nonlinearity.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/opticalbench.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/opticalbench.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/pixelbinning.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/pixelbinning.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/rawusb.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/rawusb.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/spectrometer.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/spectrometer.py`

 * *Files 1% similar despite different names*

```diff
@@ -693,7 +693,52 @@
 
 class SeaBreezeSpectrometerFeatureSR6(SeaBreezeSpectrometerFeatureOBP2):
     pass
 
 
 class SeaBreezeSpectrometerFeatureST(SeaBreezeSpectrometerFeatureOBP2):
     pass
+
+
+class SeaBreezeSpectrometerFeatureHR2(SeaBreezeSpectrometerFeatureOBP):
+    def _get_spectrum_raw(self) -> NDArray[np.uint8]:
+        timeout = int(
+            self._integration_time * 1e-3 + self.protocol.transport.default_timeout_ms
+        )
+        datastring = self.protocol.query(0x000_01C_00, timeout_ms=timeout)
+        return numpy.frombuffer(datastring, dtype=numpy.uint8)
+
+    def get_intensities(self) -> NDArray[np.float_]:
+        tmp = self._get_spectrum_raw()
+        # 32byte metadata block at beginning
+        ret = tmp[32:].view(numpy.dtype("<H")).astype(numpy.double)
+        return ret * self._normalization_value
+
+    def set_trigger_mode(self, mode: int) -> None:
+        if mode in self._trigger_modes:
+            self.protocol.send(0x000_00D_01, mode, request_ack=True)
+        else:
+            raise SeaBreezeError("Only supports: %s" % str(self._trigger_modes))
+
+    def set_integration_time_micros(self, integration_time_micros: int) -> None:
+        t_min = self._integration_time_min
+        t_max = self._integration_time_max
+        if t_min <= integration_time_micros < t_max:
+            self._integration_time = integration_time_micros
+            i_time = int(integration_time_micros / self._integration_time_base)
+            self.protocol.send(0x000_00C_01, i_time)
+        else:
+            raise SeaBreezeError(f"Integration not in [{t_min:d}, {t_max:d}]")
+
+    def get_wavelengths(self) -> NDArray[np.float_]:
+        data = self.protocol.query(0x000_011_00)
+        num_coeffs = len(data) // 4
+        assert len(data) % 4 == 0  # ???
+        assert num_coeffs > 1  # ???
+        coeffs = struct.unpack("<" + "f" * num_coeffs, data)[1:]
+        # and generate the wavelength array
+        indices = numpy.arange(self._spectrum_length, dtype=numpy.float64)
+        return sum(wl * (indices**i) for i, wl in enumerate(coeffs))  # type: ignore
+
+
+class SeaBreezeSpectrometerFeatureHR4(SeaBreezeSpectrometerFeatureOBP2):
+    pass
```

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/spectrumprocessing.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/spectrumprocessing.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/temperature.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/temperature.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/thermoelectric.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/thermoelectric.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/features/wificonfiguration.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/features/wificonfiguration.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/protocol.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/protocol.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/transport.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/transport.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/pyseabreeze/types.py` & `seabreeze-2.8.0/src/seabreeze/pyseabreeze/types.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/spectrometers.py` & `seabreeze-2.8.0/src/seabreeze/spectrometers.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze/types.py` & `seabreeze-2.8.0/src/seabreeze/types.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/src/seabreeze.egg-info/PKG-INFO` & `seabreeze-2.8.0/src/seabreeze.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seabreeze
-Version: 2.7.0
+Version: 2.8.0
 Summary: Python interface module for Ocean Optics spectrometers. This software is not associated with Ocean Optics. Use it at your own risk.
 Home-page: https://github.com/ap--/python-seabreeze
 Author: Andreas Poehlmann
 Author-email: andreas@poehlmann.io
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -62,14 +62,24 @@
 
 ```bash
 # via conda
 conda install -c conda-forge seabreeze
 seabreeze_os_setup
 ```
 
+### Using the backend pyseabreeze in Windows
+
+The backend pyseabreeze requires the libraries pyusb and libusb
+```bash
+# via pypi
+pip install seabreeze[pyseabreeze]  # this ensures installation of pyusb
+```
+Additionally, you might need to manually install libusb1. Go here https://libusb.info/, Downloads -> Latest Windows Binaries. In the zip file, enter either the folder MinGW64/dll or MinGW32/dll (depending on your OS). Copy the file `libusb-1.0.dll` into `C:\Windows\System32`.
+
+
 ## Usage
 
 The following example shows how simple it is to acquire a spectrum with
 python-seabreeze through the model independent _Spectrometer_ class. For a more
 detailed description read the [documentation](https://python-seabreeze.readthedocs.io/en/latest/):
 
 ```python
@@ -114,14 +124,16 @@
 | USB4000      |     x      |            x             |
 | USB650       |            | ap--/python-seabreeze#47 |
 | SPARK        |     x      |            x             |
 | ADC1000      |            |            x             |
 | SR2          |            |            x             |
 | SR4          |            |            x             |
 | SR6          |            |            x             |
+| HR2          |            |            x             |
+| HR4          |            |            x             |
 | ST-VIS       |            |            x             |
 
 
 ## Known Issues
 
 - USB2000 spectrometers cause `Data transfer error` due to old firmware [Issue #48](https://github.com/ap--/python-seabreeze/issues/48)
 - USB650 not supported [Issue #47](https://github.com/ap--/python-seabreeze/issues/47)
```

### Comparing `seabreeze-2.7.0/src/seabreeze.egg-info/SOURCES.txt` & `seabreeze-2.8.0/src/seabreeze.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/tests/conftest.py` & `seabreeze-2.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/tests/test_backends.py` & `seabreeze-2.8.0/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/tests/test_protocol.py` & `seabreeze-2.8.0/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `seabreeze-2.7.0/tests/test_spectrometers.py` & `seabreeze-2.8.0/tests/test_spectrometers.py`

 * *Files identical despite different names*

