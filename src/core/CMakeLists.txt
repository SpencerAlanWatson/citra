set(SRCS
            arm/disassembler/arm_disasm.cpp
            arm/disassembler/load_symbol_map.cpp
            arm/dyncom/arm_dyncom.cpp
            arm/dyncom/arm_dyncom_dec.cpp
            arm/dyncom/arm_dyncom_interpreter.cpp
            arm/dyncom/arm_dyncom_run.cpp
            arm/dyncom/arm_dyncom_thumb.cpp
            arm/interpreter/arm_interpreter.cpp
            arm/interpreter/armcopro.cpp
            arm/interpreter/armemu.cpp
            arm/interpreter/arminit.cpp
            arm/interpreter/armsupp.cpp
            arm/interpreter/armvirt.cpp
            arm/interpreter/thumbemu.cpp
            arm/skyeye_common/vfp/vfp.cpp
            arm/skyeye_common/vfp/vfpdouble.cpp
            arm/skyeye_common/vfp/vfpinstr.cpp
            arm/skyeye_common/vfp/vfpsingle.cpp
            file_sys/archive_extsavedata.cpp
            file_sys/archive_romfs.cpp
            file_sys/archive_savedata.cpp
            file_sys/archive_savedatacheck.cpp
            file_sys/archive_sdmc.cpp
            file_sys/archive_systemsavedata.cpp
            file_sys/disk_archive.cpp
            file_sys/ivfc_archive.cpp
            hle/kernel/address_arbiter.cpp
            hle/kernel/event.cpp
            hle/kernel/kernel.cpp
            hle/kernel/mutex.cpp
            hle/kernel/semaphore.cpp
            hle/kernel/shared_memory.cpp
            hle/kernel/timer.cpp
            hle/kernel/thread.cpp
            hle/service/ac_u.cpp
            hle/service/act_u.cpp
            hle/service/am_app.cpp
            hle/service/am_net.cpp
            hle/service/apt_a.cpp
            hle/service/apt_u.cpp
            hle/service/boss_u.cpp
            hle/service/cecd_u.cpp
            hle/service/cfg/cfg.cpp
            hle/service/cfg/cfg_i.cpp
            hle/service/cfg/cfg_u.cpp
            hle/service/csnd_snd.cpp
            hle/service/dsp_dsp.cpp
            hle/service/err_f.cpp
            hle/service/frd_u.cpp
            hle/service/fs/archive.cpp
            hle/service/fs/fs_user.cpp
            hle/service/gsp_gpu.cpp
            hle/service/hid_user.cpp
            hle/service/http_c.cpp
            hle/service/ir_rst.cpp
            hle/service/ir_u.cpp
            hle/service/ldr_ro.cpp
            hle/service/mic_u.cpp
            hle/service/ndm_u.cpp
            hle/service/news_u.cpp
            hle/service/nim_aoc.cpp
            hle/service/nwm_uds.cpp
            hle/service/pm_app.cpp
            hle/service/ptm_u.cpp
            hle/service/service.cpp
            hle/service/soc_u.cpp
            hle/service/srv.cpp
            hle/service/ssl_c.cpp
            hle/service/y2r_u.cpp
            hle/config_mem.cpp
            hle/hle.cpp
            hle/svc.cpp
            hw/gpu.cpp
            hw/hw.cpp
            loader/elf.cpp
            loader/loader.cpp
            loader/ncch.cpp
            loader/3dsx.cpp
            core.cpp
            core_timing.cpp
            mem_map.cpp
            mem_map_funcs.cpp
            settings.cpp
            system.cpp
            )

set(HEADERS
            arm/disassembler/arm_disasm.h
            arm/disassembler/load_symbol_map.h
            arm/dyncom/arm_dyncom.h
            arm/dyncom/arm_dyncom_dec.h
            arm/dyncom/arm_dyncom_interpreter.h
            arm/dyncom/arm_dyncom_run.h
            arm/dyncom/arm_dyncom_thumb.h
            arm/interpreter/arm_interpreter.h
            arm/skyeye_common/arm_regformat.h
            arm/skyeye_common/armcpu.h
            arm/skyeye_common/armdefs.h
            arm/skyeye_common/armemu.h
            arm/skyeye_common/armmmu.h
            arm/skyeye_common/armos.h
            arm/skyeye_common/skyeye_defs.h
            arm/skyeye_common/skyeye_types.h
            arm/skyeye_common/vfp/asm_vfp.h
            arm/skyeye_common/vfp/vfp.h
            arm/skyeye_common/vfp/vfp_helper.h
            arm/arm_interface.h
            file_sys/archive_backend.h
            file_sys/archive_extsavedata.h
            file_sys/archive_romfs.h
            file_sys/archive_savedata.h
            file_sys/archive_savedatacheck.h
            file_sys/archive_sdmc.h
            file_sys/archive_systemsavedata.h
            file_sys/disk_archive.h
            file_sys/file_backend.h
            file_sys/ivfc_archive.h
            file_sys/directory_backend.h
            hle/kernel/address_arbiter.h
            hle/kernel/event.h
            hle/kernel/kernel.h
            hle/kernel/mutex.h
            hle/kernel/semaphore.h
            hle/kernel/session.h
            hle/kernel/shared_memory.h
            hle/kernel/timer.h
            hle/kernel/thread.h
            hle/service/ac_u.h
            hle/service/act_u.h
            hle/service/am_app.h
            hle/service/am_net.h
            hle/service/apt_a.h
            hle/service/apt_u.h
            hle/service/boss_u.h
            hle/service/cecd_u.h
            hle/service/cfg/cfg.h
            hle/service/cfg/cfg_i.h
            hle/service/cfg/cfg_u.h
            hle/service/csnd_snd.h
            hle/service/dsp_dsp.h
            hle/service/err_f.h
            hle/service/frd_u.h
            hle/service/fs/archive.h
            hle/service/fs/fs_user.h
            hle/service/gsp_gpu.h
            hle/service/hid_user.h
            hle/service/http_c.h
            hle/service/ir_rst.h
            hle/service/ir_u.h
            hle/service/ldr_ro.h
            hle/service/mic_u.h
            hle/service/ndm_u.h
            hle/service/news_u.h
            hle/service/nim_aoc.h
            hle/service/nwm_uds.h
            hle/service/pm_app.h
            hle/service/ptm_u.h
            hle/service/service.h
            hle/service/soc_u.h
            hle/service/srv.h
            hle/service/ssl_c.h
            hle/service/y2r_u.h
            hle/config_mem.h
            hle/result.h
            hle/function_wrappers.h
            hle/hle.h
            hle/svc.h
            hw/gpu.h
            hw/hw.h
            loader/elf.h
            loader/loader.h
            loader/ncch.h
            loader/3dsx.h
            core.h
            core_timing.h
            mem_map.h
            settings.h
            system.h
            )

create_directory_groups(${SRCS} ${HEADERS})

add_library(core STATIC ${SRCS} ${HEADERS})
