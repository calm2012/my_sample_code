# 构建说明：
1. 代码根目录创建debug目录
2. 进入debug
3. cmake生成VS工程文件
```cmake
cmake ../ -DCMAKE_BUILD_TYPE=Debug -G "Visual Studio 16 2019" -A x64
```
- 注意：cmake编译参数请添加参数： -A x64 生成x64工程（由于附带的GoogleTest库位x64版本，所以32位工程会编译不过，然然如果使用自己编译的GoogleTest则不受此限制。）
- 推荐使用：Visual Studio 16 2019