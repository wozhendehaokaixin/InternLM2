### 作业（七）

本节课主要使用OpenCompass评测工具

##### 列出所有跟 InternLM 及 C-Eval 相关的配置：

![屏幕截图 2024-04-27 131415](C:\Users\27111\Desktop\课7\屏幕截图 2024-04-27 131415.png)

##### 出现错误情况：

![屏幕截图 2024-04-27 134245](C:\Users\27111\Desktop\课7\屏幕截图 2024-04-27 134245.png)

##### 运行时错误信息：

出现InternLM2Converter requires the protobuf library...解决方案：

```
pip install protobuf
```

遇到错误mkl-service + Intel(R) MKL MKL_THREADING_LAYER=INTEL is incompatible with libgomp.so.1 ... 

![屏幕截图 2024-04-27 134225](C:\Users\27111\Desktop\课7\屏幕截图 2024-04-27 134225.png)

解决方案：

```
export MKL_SERVICE_FORCE_INTEL=1
#或
export MKL_THREADING_LAYER=GNU
```

##### 正确评测结果：

![屏幕截图 2024-04-27 151650](C:\Users\27111\Desktop\课7\屏幕截图 2024-04-27 151650.png)

![屏幕截图 2024-04-27 151706](C:\Users\27111\Desktop\课7\屏幕截图 2024-04-27 151706.png)