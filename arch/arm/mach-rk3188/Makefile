EXTRA_CFLAGS += -Os
ifneq ($(CONFIG_RK_FPGA),y)
obj-y += clock_data.o
endif
ifneq ($(CONFIG_ARCH_RK30XX),y)
obj-$(CONFIG_CPU_FREQ) += cpufreq.o
endif
CFLAGS_common.o += -DTEXT_OFFSET=$(TEXT_OFFSET)
obj-y += io.o
obj-y += rk_timer.o
obj-$(CONFIG_CPU_FREQ) += cpufreq.o
obj-$(CONFIG_DVFS) += dvfs.o
obj-y += board.o

board-$(CONFIG_MACH_RK3188_FPGA) += board-rk3188-fpga.o
board-$(CONFIG_MACH_RK3188_DS1006H) += board-rk3188-ds1006h.o
