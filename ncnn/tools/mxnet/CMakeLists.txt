# add this two lines
set(Protobuf_INCLUDE_DIR /home/dongbin/anaconda3/envs/ncnn/include)
set(Protobuf_LIBRARY /home/dongbin/anaconda3/envs/ncnn/lib/libprotobuf.so)

add_executable(mxnet2ncnn mxnet2ncnn.cpp)

# add all mxnet2ncnn tool to a virtual project group
set_property(TARGET mxnet2ncnn PROPERTY FOLDER "tools/converter")
