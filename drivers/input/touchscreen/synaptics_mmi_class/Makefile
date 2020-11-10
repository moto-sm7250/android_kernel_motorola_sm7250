#
# Makefile for the Synaptics DSX touchscreen driver.
#

ifneq ($(filter m y,$(CONFIG_INPUT_TOUCHSCREEN_MMI)),)
	ccflags-y += -DCONFIG_INPUT_TOUCHSCREEN_MMI
endif

# Each configuration option enables a list of files.
synaptics_mmi-y += synaptics_dsx_i2c.o synaptics_mmi_class.o synaptics_dsx_instance.o
obj-$(CONFIG_TOUCHSCREEN_SYNAPTICS_DSX_MMI_CORE) += synaptics_mmi.o
obj-$(CONFIG_TOUCHSCREEN_SYNAPTICS_DSX_MMI_RMI_DEV) += synaptics_dsx_rmi_dev.o
obj-$(CONFIG_TOUCHSCREEN_SYNAPTICS_DSX_MMI_FW_UPDATE) += synaptics_dsx_fw_update.o
obj-$(CONFIG_TOUCHSCREEN_SYNAPTICS_DSX_MMI_TEST_REPORTING) += synaptics_dsx_test_reporting.o
