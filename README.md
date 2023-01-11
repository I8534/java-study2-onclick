# java-study2-1


  <div class="box-wrapper">
    <div class="box">
      <p>BOX</p>
      <button onclick="Box('none')" class="close-btn">x</button>
    </div>
  </div>

  <button onclick="Box('block')" class="open-btn">open</button>

여기에서 온클릭을 통해서 각각의 함수 안에 넣을 것을 정했다.

그 다음 javascript에서 

function Box(para) {
  document.querySelector('.box-wrapper').style.display = para;
  // 빈박스이고 
}

이렇게 입력하자. 그러면 Box라는 함수에서 display를 매개변수로 두고 있고 

document.querySelector('.box-wrapper').style.display라는 식은 Box(para)의 display 값을 입력받는 것이다. 

즉 위의 html의 onclick="Box('block')" 식을 입력하기 전에 이 para라는 것은 빈 박스였다.

그러나 onclick="Box('block')"  onclick="Box('none')" 을 입력함으로서 매개변수인 para에

'block'와 'none'이 입력이 되는 것이다.

다른 자바 코드와 다르게 함수가 선언이 안 된 것은 온클릭을 통해 간접적으로 함수 선언을 하기 때문이다.




