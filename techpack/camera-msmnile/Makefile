# SPDX-License-Identifier: GPL-2.0-only

# auto-detect subdirs
ifeq ($(CONFIG_ARCH_SM8150), y)
include $(srctree)/techpack/camera-msmnile/config/msmnilecamera.conf
endif

ifeq ($(CONFIG_ARCH_SM8150), y)
LINUXINCLUDE    += \
		-include $(srctree)/techpack/camera-msmnile/config/msmnilecameraconf.h
endif

# auto-detect subdirs
ifeq ($(CONFIG_MACH_XIAOMI_CEPHEUS), y)
include $(srctree)/techpack/camera-msmnile/config/cepheus.conf
endif

ifeq ($(CONFIG_MACH_XIAOMI_CEPHEUS), y)
LINUXINCLUDE    += \
		-include $(srctree)/techpack/camera-msmnile/config/cepheus.h
endif

# auto-detect subdirs
ifeq ($(CONFIG_MACH_XIAOMI_CRUX), y)
include $(srctree)/techpack/camera-msmnile/config/crux.conf
endif

ifeq ($(CONFIG_MACH_XIAOMI_CRUX), y)
LINUXINCLUDE    += \
		-include $(srctree)/techpack/camera-msmnile/config/crux.h
endif

# auto-detect subdirs
ifeq ($(CONFIG_MACH_XIAOMI_ANDROMEDA), y)
include $(srctree)/techpack/camera-msmnile/config/crux.conf
endif

ifeq ($(CONFIG_MACH_XIAOMI_ANDROMEDA), y)
LINUXINCLUDE    += \
		-include $(srctree)/techpack/camera-msmnile/config/crux.h
endif

ifdef CONFIG_SPECTRA_CAMERA_MSMNILE
# Use USERINCLUDE when you must reference the UAPI directories only.
USERINCLUDE     += \
                -I$(srctree)/techpack/camera-msmnile/include/uapi

# Use LINUXINCLUDE when you must reference the include/ directory.
# Needed to be compatible with the O= option
LINUXINCLUDE    += \
                -I$(srctree)/techpack/camera-msmnile/include/uapi \
                -I$(srctree)/techpack/camera-msmnile/include
obj-y += drivers/
endif
