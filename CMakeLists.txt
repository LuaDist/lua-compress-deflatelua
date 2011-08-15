# Copyright (C) 2011 LuaDist.
# Created by Peter Kapec
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

PROJECT (lua-compress-deflatelua NONE)
CMAKE_MINIMUM_REQUIRED (VERSION 2.6)
INCLUDE ( dist.cmake )

# Install all files and documentation
install_lua_module ( compress.deflatelua module/lmod/compress/deflatelua.lua )
install_lua_module ( bin.gunziplua module/lmod/bin/gunziplua.lua )

install_lua_executable( gunziplua bin/gunziplua)

install_test(test/test.lua)
install_data ( COPYRIGHT  share/compress.deflatelua/hello.txt.gz  )




