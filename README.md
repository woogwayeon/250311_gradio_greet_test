# 250311_gradio_greet_test
그라디오를 이용한 간단한 인사 프로그램을 제작했습니다

## Greet 프로그램

---

```
import gradio as gr

def greet(name):
  return "hello" + name + '!'

demo = gr.Interface(fn=greet, inputs="text", outputs="text")

# 디버그 체크해보자
demo.launch(debug=True, share=True)
```

그라디오를 임포트해오고 greet라는 함수 만들어줌

데모로 그라디오에 있는 Interface함수? 에다가 텍스트를 넣었따!

이름넣고 제출하면 `hello seoyeon!` 이 출력된다

그리고 `demo.lanch()` 를 사용해서 찍어보았다



참고로 저 서버는 3일동안만 살아있으니까 포폴로 쓸거면 면접할때 다시 실행시키고 가든 하자..
