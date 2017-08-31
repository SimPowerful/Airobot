# Airobot
Home service robots
############################## 描述
This is ouer home service robot code by ROS!

1.Drivers
   ROS arduino bridge,use mega2560 mcu,two pwm output driver for motor ,PID ctrl, ... ...
   
2.SLAM
   kinect 2.0 ... ...
   
3.Speech Recognition and Synthesis
   xunfei ... ...
############################## github
#upload上传数据
git add .
git commit -m "修改记录"
git push origin master
#updata更新数据
git pull
############################## 重要网页收藏
http://www.ncnynl.com/archives/201702/1287.html  //讯飞在线语音合成和识别  


############################## 命令说明
#讯飞在线语音合成和识别
rosrun xfei_asr  tts_subscribe_speak
rostopic pub xfwords std_msgs/String "测试ncnynl.com"

rosrun xfei_asr  iat_publish_speak
rostopic echo /xfspeech
rostopic echo /xfwords
rostopic pub xfwakeup std_msgs/String "ok"


















