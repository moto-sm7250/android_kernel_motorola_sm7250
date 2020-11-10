ifneq ($(filter m y,$(CONFIG_INPUT_TOUCHSCREEN_MMI)),)
	ccflags-y += -DCONFIG_INPUT_TOUCHSCREEN_MMI
endif

goodix_v1430_mmi-y += goodix_ts_i2c.o goodix_ts_core.o goodix_cfg_bin.o
goodix_v1430_mmi-$(CONFIG_TOUCHSCREEN_GOODIX_GTX8_MMI_GESTURES) += goodix_ts_mmi.o
obj-$(CONFIG_TOUCHSCREEN_GOODIX_GTX8_MMI) += goodix_v1430_mmi.o
goodix_v1430_update_mmi-y += goodix_gtx8_update.o
obj-$(CONFIG_TOUCHSCREEN_GOODIX_GTX8_MMI_UPDATE) += goodix_v1430_update_mmi.o
goodix_v1430_ts_tools_mmi-y += goodix_ts_tools.o
obj-$(CONFIG_TOUCHSCREEN_GOODIX_GTX8_MMI_TOOLS) += goodix_v1430_ts_tools_mmi.o
