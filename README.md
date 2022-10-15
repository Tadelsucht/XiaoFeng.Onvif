# ��ӭʹ�� XiaoFeng.Onvif ���߿�

** �������Ŀ�����nuget�����ã����� XiaoFeng.Onvif  **

####�����÷�
```
using XiaoFeng.Onvif;

var ip = "192.168.12.2";
var user = "onvif";
var pass = "123456";

var onvifUTCDateTime = await DeviceService.GetSystemDateAndTime(ip);
var info= await DeviceService.GetDeviceInformation(ip, user, pass, onvifUTCDateTime);
var  capabilities= await DeviceService.GetCapabilities(ip);
var tokens = await MediaService.GetProfiles(ip, user, pass, onvifUTCDateTime);
var streamUri = await MediaService.GetStreamUri(ip, user, pass, onvifUTCDateTime, tokens[0]);
var img =  await MediaService.GetSnapshotUri(ip, user, pass, onvifUTCDateTime, tokens[0]);
var status=  await PTZService.GetStatus(ip, user, pass, onvifUTCDateTime, tokens[0]);

```

####��Դ����
�ڵ���Onvif��װ���ߵ�ʱ�򣬷���.NET ���������п�Դ��onvif��Ŀ���е���Ŀ���Ǹ��ѵġ���ʱ����onvif����ļ�����Ա���ʱ���˼�ֱ��˵��Դ���շ�xxxxԪ��

�������ļ��ҵ������������Լ��з���һ��.NET Core��Դ����Ŀ������Ŀ���ڿ�Դ���������ܶ������ˣ���Ȼ���Լ��ľ��������޵ģ�����ʰ�����ߣ�ϣ��������Ƶ�������Ȥ��С���һ�����ɣ�

��������ʵ����ػ������ܣ����ڿ������ɷ������ϵͳ��ϣ��ͨ������һ��������.NET����������Ƶ����ļ�����

####����Ŀ��Դ100%���
####����Ŀ��Դ100%���
####����Ŀ��Դ100%���
��Դ���ף�·����С�����Ը�С����github�����С���ǣ��Դ˼���һ��С�࣡

####��ϵ��
��Ϊgithub��������ȷʵ�������˸��´��룬���˷���githubƵ��Ҳ�ͣ���������ʵ�С�����Թ�ע���ںţ�������ϵ




