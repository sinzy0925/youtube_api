# youtube_api

# 使い方１（python実行環境が有る人向け）
- ```python youtube_apiA.py``` で起動すると、
- ```localhost:8001```で起動します。
- ブラウザに ```http://localhost:8001``` と入力してエンターして、
- {"status":"ok","message":"API is running"}と表示されれば起動OKです。

# 使い方２（python実行環境が無い人向け）
- distフォルダにある、
- ```youtube_apiA.exe```をダブルクリックして起動すると上記と同じく 
- ```localhost:8001```で起動します。
- ブラウザに ```http://localhost:8001``` と入力してエンターして、
- {"status":"ok","message":"API is running"}と表示されれば起動OKです。

# 使い方３（字幕取得方法）
- ```http://localhost:8001/transcript?videoId=???```
- 上記URLの最後???に取得したいyoutubeのURLのv=の右側を入れてブラウザで実行します。
###
- この字幕を取得するなら```https://www.youtube.com/watch?v=O_bmmDWIjTc```
###
- ```http://localhost:8001/transcript?videoId=O_bmmDWIjTc``` と入力します。
###
- 出力は以下の通りJSONです。
- {"text":transcript,"lang":detected_lang,"text_time":transcript_time,"now_jst":now_jst.strftime("%Y-%m-%d %H:%M:%S"),"text_time_duration":transcript_all}



