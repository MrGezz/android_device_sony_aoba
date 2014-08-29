android_device_sony_aoba
========================

Sony Xperia Ion (OpenSEMC)
 Device tree for sony xperia Ion, Aoba

The ril for Xperia Ion (aoba) is not fixed because of cleaning blob, I'm just randomly making that commit because I'm still a newbie during that time, there are some correction here:

add this line "rild.libpath=/system/lib/libril-qc-qmi-1.so" to system.prop without the quotes

and lastly , add this in full_aoba.mk

"# Inherit from those products. Most specific first.
$(call inherit-product, $(SRC_TARGET_DIR)/product/full_base_telephony.mk)"

and of course without the quotes too.
the line above essential to enable telephony
