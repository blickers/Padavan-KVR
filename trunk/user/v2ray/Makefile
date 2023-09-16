THISDIR = $(shell pwd)
v2ray_dir="v2ray.com/core/main"
export GO111MODULE=on
export GOPROXY=https://goproxy.cn
V2ray_VERSION := 5.7.0
V2ray_URL := https://codeload.github.com/v2fly/v2ray-core/tar.gz/v$(V2ray_VERSION)
V2RAY_SED_ARGS:=
V2RAY_SED_ARGS += \
	s/_ "v2ray.com\/core\/main\/json"/\/\/ &/; \
	/\/\/ _ "v2ray.com\/core\/main\/jsonem"/s/\/\/ //;
V2RAY_SED_ARGS += \
	s/_ "v2ray.com\/core\/main\/json"/\/\/ &/;

all:download_v2 build_extract build_v2ray
#all:download_v2 

download_v2:


build_extract:


build_v2ray:


clean:
	#rm -rf $(THISDIR)/v2ray.com
	#rm -rf $(THISDIR)/bin

romfs:
	$(ROMFSINST) -p +x $(THISDIR)/v2ray /usr/bin
