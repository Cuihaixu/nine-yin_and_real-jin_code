
THEOS_DEVICE_IP = 127.0.0.1
THEOS_DEVICE_PORT = 2222
ARCHS = armv7 arm64

include $(THEOS)/makefiles/common.mk

TWEAK_NAME = preferencestweak
preferencestweak_FILES = Tweak.xm

preferencestweak_LDFLAGS = -lMobileGestalt

include $(THEOS_MAKE_PATH)/tweak.mk

after-install::
	install.exec "killall -9 Preferences"
