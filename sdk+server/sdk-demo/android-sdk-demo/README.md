������� Android sdk ʾ�� demo
===

### demo ���в���

* 1������ģ��ҵ���ˣ�check demo�����з�����activity-protection-check-demoĿ¼

* 2���޸� MainActivity.java �� onCreate���������� productNumber�����£�
```
     watchman.init(getApplicationContext(), "your productNumber");
```	 
* 3���޸� ActivityTask.java�� doInBackground ����,�� params.put()����������BusinessId,���£�
```
	 params.put("token", watchman.getToken("your BusinessId"));
```
* 4���޸� ActivityTask.java�� PostData�����е�url����
```
     String url = "http://localhost:8181/rise.do";
     // ���磬�滻���£�
     String url = "http://10.240.132.43:8181/rise.do";
```
* 5�����ˣ����ú��޸���ɣ��������м���