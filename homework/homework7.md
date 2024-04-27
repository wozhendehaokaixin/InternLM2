### 作业（七）

本节课主要使用OpenCompass评测工具

##### 列出所有跟 InternLM 及 C-Eval 相关的配置：

![屏幕截图 2024-04-27 131415](https://github.com/wozhendehaokaixin/InternLM2/raw/main/png/%E8%AF%BE7/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202024-04-27%20131415.png)

##### 出现错误情况：

![屏幕截图 2024-04-27 134245](https://github.com/wozhendehaokaixin/InternLM2/raw/main/png/%E8%AF%BE7/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202024-04-27%20134245.png)

##### 运行时错误信息：

出现InternLM2Converter requires the protobuf library...解决方案：

```
pip install protobuf
```

遇到错误mkl-service + Intel(R) MKL MKL_THREADING_LAYER=INTEL is incompatible with libgomp.so.1 ... 

![屏幕截图 2024-04-27 134225](https://github.com/wozhendehaokaixin/InternLM2/raw/main/png/%E8%AF%BE7/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202024-04-27%20134225.png)

解决方案：

```
export MKL_SERVICE_FORCE_INTEL=1
#或
export MKL_THREADING_LAYER=GNU
```

##### 正确评测结果：

![屏幕截图 2024-04-27 151650](https://github.com/wozhendehaokaixin/InternLM2/raw/main/png/%E8%AF%BE7/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202024-04-27%20151650.png)

![屏幕截图 2024-04-27 151706](https://github.com/wozhendehaokaixin/InternLM2/raw/main/png/%E8%AF%BE7/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202024-04-27%20151706.png)
