InspectLua
==========

主要深入学习Lua，包括Lua与C等其他语言的交互、Lua源码阅读等。下面是各个源文件一个简单的说明：

学习在C中调用lua的一般全局变量、table以及函数相应的文件有：

    TestConfig.lua 
    
    util.h
    
    util.c                                --主要定义了打印lua栈、C中调用Lua的函数一个通用接口
    capi_example.c                        --主要用来熟悉lua与c交互的一些API
    c_function_to_extend_lua.c
    extend_c_app_by_lua.c
    test_general_call_lua_in_c.c
    simple_lua_interpreter.c

学习在Lua中使用C中定义的函数、模块以及userdata，相关的文件有：

    TestLuaExtendedbyC.lua
    
    c_function_to_extend_lua.h
    
    c_function_to_extend_lua.c
    c_module_to_extend_lua.c
    c_userdata_to_extend_lua.c
    c_userdata_with_gc_to_extend_lua.c      --测试lua在回收userdata时，会调用相应元表的__gc对应方法
    test_extend_lua_by_c.c
    
把C++中定义的类以及成员方法，在lua中使用，相关的文件有:

    TestBindingCppWithLua.lua
    
    binding_cpp_with_lua.cpp
    binding_cpp_with_lua.hpp        --定义了模板，可以方便封装要在lua中使用的类以及方法
    test_binding_cpp_with_lua.hpp
    
利用LuaBridge绑定C++到Lua，相关的文件有：

    LuaBridge/             
    study_lua_bridge_main.cpp  
    study_lua_bridge.lua
    
利用LuaBridge绑定C++到Lua，相关的文件有：

    TestBindingCppWithLua.lua
    test_binding_cpp_with_lua.cpp
    binding_cpp_with_lunafive.hpp
    
利用lunar绑定C++到Lua，相关的文件有：

    lunar_test_script.lua
    lunar_test_main.cpp
    lunar.hpp


