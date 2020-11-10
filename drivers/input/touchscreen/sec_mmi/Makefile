sec_mmi-y += sec_ts.o sec_ts_fn.o sec_ts_fw.o sec_cmd.o sec_ts_only_vendor.o

ifneq ($(filter m y,$(CONFIG_INPUT_TOUCHSCREEN_MMI)),)
    ccflags-y += -DCONFIG_INPUT_TOUCHSCREEN_MMI
    ccflags-y += -DCONFIG_PANEL_NOTIFICATIONS
    sec_mmi-y += sec_ts_mmi_class.o
else
    ccflags-y += -DUSE_STUBS
    sec_mmi-y += sec_ts_mmi.o
endif

obj-$(CONFIG_TOUCHSCREEN_SEC_TS) += sec_mmi.o
