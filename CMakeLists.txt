cmake_minimum_required(VERSION 3.20.0)

find_package(Zephyr)
project(app_test)

target_sources(app PRIVATE src/main.c src/test_module.c)
#target_sources_ifdef(CONFIG_SHELL_DYNAMIC_CMDS app PRIVATE src/dynamic_cmd.c)
#target_sources_ifdef(CONFIG_SHELL_BACKEND_SERIAL app PRIVATE src/uart_reinit.c)
#target_sources_ifdef(CONFIG_SHELL_START_OBSCURED app PRIVATE src/login_cmd.c)
