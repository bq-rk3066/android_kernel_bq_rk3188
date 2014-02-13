EXTRA_CFLAGS += -Os
ifneq ($(CONFIG_RK_FPGA),y)
obj-y += clock_data.o
obj-y += ddr.o
obj-y += pmu.o
obj-y += reset.o
obj-$(CONFIG_PM) += pm.o
endif
obj-y += common.o
ifneq ($(CONFIG_ARCH_RK30XX),y)
obj-$(CONFIG_CPU_FREQ) += cpufreq.o
endif
CFLAGS_common.o += -DTEXT_OFFSET=$(TEXT_OFFSET)
obj-y += devices.o
obj-y += io.o
obj-y += rk_timer.o
obj-$(CONFIG_SMP) += platsmp.o headsmp.o
obj-$(CONFIG_HOTPLUG_CPU) += hotplug.o
obj-$(CONFIG_CPU_IDLE) += cpuidle.o
obj-$(CONFIG_CPU_FREQ) += cpufreq.o
obj-$(CONFIG_DVFS) += dvfs.o

obj-$(CONFIG_SOC_RK3108) += board.o
board-$(CONFIG_MACH_RK3108_TB) += board-rk3108-tb.o

obj-$(CONFIG_SOC_RK3168) += board.o
board-$(CONFIG_MACH_RK3168_TB) += board-rk3168-tb.o
board-$(CONFIG_MACH_RK3168_LR097) += board-rk3168-LR097.o
board-$(CONFIG_MACH_RK3168_DS1006H) += board-rk3168-ds1006h.o
board-$(CONFIG_MACH_RK3168_86V) += board-rk3168-86v.o
board-$(CONFIG_MACH_RK3168_86V_OLD) += board-rk3168-86v-old.o

obj-$(CONFIG_SOC_RK3168M) += board.o
board-$(CONFIG_MACH_RK3168M_TB) += board-rk3168m-tb.o

obj-$(CONFIG_SOC_RK3188) += board.o
board-$(CONFIG_MACH_RK3188_FPGA) += board-rk3188-fpga.o
board-$(CONFIG_MACH_RK3188_TB) += board-rk3168-tb.o
board-$(CONFIG_MACH_RK3188_LR097) += board-rk3168-LR097.o
board-$(CONFIG_MACH_RK3188_DS1006H) += board-rk3188-ds1006h.o
board-$(CONFIG_MACH_RK3188_PHONEPAD) += board-rk3168-phonepad.o
