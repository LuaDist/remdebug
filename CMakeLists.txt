# Copyright (C) 2007-2009 LuaDist.
# Created by Peter Drahoš
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

PROJECT(remdebug NONE)
CMAKE_MINIMUM_REQUIRED(VERSION 2.6)
INCLUDE(dist.cmake)

# RemDebug modules
INSTALL (FILES src/remdebug/engine.lua DESTINATION ${INSTALL_LMOD}/remdebug)
INSTALL (FILES src/controller.lua DESTINATION ${INSTALL_LMOD})

# Install RemDebug documentation
INSTALL(DIRECTORY doc/ DESTINATION ${INSTALL_DOC})
INSTALL(DIRECTORY tests/ DESTINATION ${INSTALL_TEST})
