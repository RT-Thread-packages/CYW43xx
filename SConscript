import rtconfig
Import('RTT_ROOT')
from building import *

# get current directory
cwd = GetCurrentDir()
path = []
src = []

# The set of source files associated with this SConscript file.
path += [
    cwd + '/cyw43-driver/src',
    cwd + '/cyw43-driver/firmware',
]
src += [
    cwd + '/cyw43-driver/src/cyw43_ctrl.c',
    cwd + '/cyw43-driver/src/cyw43_ll.c',
    cwd + '/cyw43-driver/src/cyw43_lwip.c',
    cwd + '/cyw43-driver/src/cyw43_sdio.c',
    cwd + '/cyw43-driver/src/cyw43_stats.c',
]

group = DefineGroup('cyw43-driver', src, depend = [''], CPPPATH = path)

Return('group')