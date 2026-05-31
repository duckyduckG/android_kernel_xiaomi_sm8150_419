vendor := $(srctree)/$(src)

ifneq "$(wildcard $(vendor)/qcom)" ""
	subdir-y += qcom
endif

ifneq "$(wildcard $(vendor)/qcom_legacy)" ""
	subdir-y += qcom_legacy
endif
