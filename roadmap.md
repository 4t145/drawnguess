# 服务端
一个room 2-8个人

base on rust
powered by tokio

## 消息类型
## 房间服务


# Web
## canvas
判断鼠标位置

# 编码
编码采用一秒30帧，每10帧一组的方式
第一帧是关键帧，之后每一帧是相对于之前的改变（采用覆盖的方式）
```
KeyFrameSize:   2                   Byte(s)
KeyFrame:       {KeyFrameSize}      Byte(s)
FollowsSize:    2                   Byte(s)

FrameSize:      2                   Byte(s)

Color:          4                   Byte(s)
CoorNums:       4                   Byte(s)
Coor:           {CoorNums}*2        Byte(s)

Color:          4                   Byte(s)
CoorNums:       4                   Byte(s)
Coor:           {CoorNums}*2        Byte(s)

.
.
.
```

# 通信
通信采用二进制格式

