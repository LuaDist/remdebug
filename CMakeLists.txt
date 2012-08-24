# Copyright (C) 2007-2009 LuaDist.
# Created by Peter Drahoš
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

project ( remdebug NONE )
cmake_minimum_required ( VERSION 2.8 )
include ( cmake/dist.cmake )
include ( lua )

# RemDebug modules
install_lua_module ( remdebug.engine src/remdebug/engine.lua )
install_lua_module ( controller controller.lua )

# Install RemDebug documentation
install_doc ( doc/ )
install_test ( tests/ )
