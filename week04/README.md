- 변수, 인자, 조건문으로 셸 스크립트 작성
- tar로 압축하고 복원한 뒤 diff로 원본과 비교
- 종료 코드(`$?`): 0은 성공, 그 외는 실패
- .gitignore로 백업 결과물은 Git에서 제외

```bash
./backup.sh test
tar -tzf <백업파일>
diff -rq test restore-check/test
```

