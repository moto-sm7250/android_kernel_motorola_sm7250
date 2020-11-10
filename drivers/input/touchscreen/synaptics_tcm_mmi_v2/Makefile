#
# Makefile for the Synaptics TCM touchscreen driver.
#

ifneq ($(filter m y,$(CONFIG_INPUT_TOUCHSCREEN_MMI)),)
	ccflags-y += -DCONFIG_INPUT_TOUCHSCREEN_MMI
endif

# Each configuration option enables a list of files.
obj-$(CONFIG_TOUCHSCREEN_SYNAPTICS_TCM_MMI_SPI) += synaptics_spi.o
obj-$(CONFIG_TOUCHSCREEN_SYNAPTICS_TCM_MMI_I2C) += synaptics_i2c.o
synaptics_core_module-y += synaptics_core.o synaptics_touch.o
synaptics_core_module-$(CONFIG_TOUCHSCREEN_SYNAPTICS_TCM_MMI_GESTURES) += synaptics_ts_mmi.o
obj-$(CONFIG_TOUCHSCREEN_SYNAPTICS_TCM_MMI_CORE) += synaptics_core_module.o
obj-$(CONFIG_TOUCHSCREEN_SYNAPTICS_TCM_MMI_DEVICE) += synaptics_device.o
obj-$(CONFIG_TOUCHSCREEN_SYNAPTICS_TCM_MMI_DIAGNOSTICS) += synaptics_diagnostics.o
obj-$(CONFIG_TOUCHSCREEN_SYNAPTICS_TCM_MMI_RECOVERY) += synaptics_recovery.o
obj-$(CONFIG_TOUCHSCREEN_SYNAPTICS_TCM_MMI_REFLASH) += synaptics_reflash.o
obj-$(CONFIG_TOUCHSCREEN_SYNAPTICS_TCM_MMI_TESTING) += synaptics_testing.o
obj-$(CONFIG_TOUCHSCREEN_SYNAPTICS_TCM_MMI_ZEROFLASH) += synaptics_zeroflash.o
