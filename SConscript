import rtconfig
Import('RTT_ROOT')
from building import *

# get current directory
cwd = GetCurrentDir()
path = []
src = []

# The set of source files associated with this SConscript file.
path += [
    cwd + '/src',
    cwd + '/firmware',
]
src += [
    cwd + '/src/cyw43_ctrl.c',
    cwd + '/src/cyw43_ll.c',
    cwd + '/src/cyw43_lwip.c',
    cwd + '/src/cyw43_sdio.c',
    cwd + '/src/cyw43_stats.c',
]

group = DefineGroup('cyw43-driver', src, depend = ['PKG_USING_CYW43XX'], CPPPATH = path)

Return('group')
