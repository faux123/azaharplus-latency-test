# AzaharPlus 2126.2-A + Azahar input lag fixes (test build)

test build I ran on my Retroid Pocket Duo, here with its source for GPLv3

base is AzaharPlus 2126.2-A (cf9068844)
added upstream Azahar #2706, #2755, and the Vulkan part of #2700
the fixes are all the Azahar devs' work, I only carried them over and measured them

about 1 frame less input lag on the Duo, 123 ms down to 104 ms

the APK installs next to your normal AzaharPlus (package `io.github.lime3ds.android.debug`), arm64 only, debug signed

not maintained, no support.. use upstream Azahar 2127.0+ (has the fixes) or AzaharPlus once it picks them up

files are on the Releases page:
- `azaharplus-2126.2-A-faux-latency-arm64.apk`
- `azaharplus-2126.2-A-faux-latency-src.tar.gz` (full source with submodules, branch `faux-latency-prs` at 8602fc4c2)
- `SHA256SUMS`

build: `cd src/android && FAUX_VC=34300010 ./gradlew assembleVanillaRelWithDebInfoLite`

license GPLv3, see LICENSE.txt
