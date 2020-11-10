ifneq ($(filter m y, $(CONFIG_TOUCHCLASS_MMI_GESTURE_POISON_EVENT)),)
	ccflags-y += -DTS_MMI_TOUCH_GESTURE_POISON_EVENT
endif

touchscreen_mmi-y += touchscreen_mmi_class.o touchscreen_mmi_panel.o touchscreen_mmi_notif.o touchscreen_mmi_gesture.o

obj-$(CONFIG_INPUT_TOUCHSCREEN_MMI) += touchscreen_mmi.o
