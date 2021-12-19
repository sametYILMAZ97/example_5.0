React ta iç içe olmasıyla 1, 2 ve 3 component olsun 1 den 3 e veri iletemiyorum
	önce 2 ye sonra 3 e veri iletebilirim.
	Bu sorun daha sonra ReactRedux ile çözülebiliyormuş.
	Bir component içerisinde değişiklik yaparsam sadece o component
	render(yeniden oluşturuluyor) ediliyor. Hız olarak çok daha iyi bir sonuç veriyor.
	JSX yapısı ile HTML kodlarıymış gibi kod yazabiliyoruz bu da öğrenebilirliği arttırıyor.
	Class compenent ile render dışında yazılmış bir function'ı render içinde çağırabiliyorum.
	index.js içerisinde App.js içeriğini HTML sayfasında root olan alana içeriği render et komutu yer alıyor.
	Bootstrap sayfayı 12 eşit row parçasına ayırıyor.
  
  
  # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
  Functional Component: 
		Sadece ekranda belirli bir miktar içerik göstermek için kullanılır.(?)
		HTTP isteği gönderilmez.
		LifeCycle metotlarına ulaşılmaz.
		State ulaşılmaz.(?) (useState)
		Yazması, okunması ve test edilmesi daha kolay.
		Daha az kod yazılarak oluşturulur.
		Performansı daha iyi.
		Örnek:
			import React, { useState } from 'react';
 
			function Example() {
			  // Declare a new state variable, which we'll call "count"
			  const [count, setCount] = useState(0);
			 
			  return (
				<div>
				  <p>You clicked {count} times</p>
				  <button onClick={() => setCount(count + 1)}>
					Click me
				  </button>
				</div>
			  );
			}
      
  # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
  Class Based Component:
		HTTP isteği gönderilir.
		Bütün veri işlemelerde kullanılır.(?)
		LifeCycle metotlarına ulaşılır.
		State ulaşılır.(?) (useState)
		Daha fazla kod yazmamız gerekir.
