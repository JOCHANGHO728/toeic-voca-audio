# toeic-voca-audio

TOEIC VOCA 앱의 **영국식·호주식 발음 녹음 묶음**을 내려주는 저장소입니다. 코드는 없고 Release `packs`의 파일만 씁니다.

- 앱의 설정 › 음성 다운로드에서 억양을 받으면 `https://github.com/JOCHANGHO728/toeic-voca-audio/releases/download/packs/` 아래의
  `index.json`(목록·크기·판)과 `voice-<언어>-<성별>.zip`(단어+예문 mp3)을 받습니다. 미국식은 앱에 들어 있습니다.
- 녹음은 Google Cloud Text-to-Speech(Chirp 3 HD)로 만든 것입니다.
- 왜 여기에 두나: 한국에서 Cloudflare 무료 서비스(r2.dev·Workers)는 미국(LAX)을 거쳐 초당 16~160KB밖에 나오지 않았고, GitHub Releases는 초당 약 9.7MB였습니다.
- 올리는 방법: 앱 저장소에서 `python content/scripts/upload_audio.py --github`
