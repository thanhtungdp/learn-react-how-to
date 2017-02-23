React là library javascript dành cho việc xây dựng UI (User interface tạm dịch gọi là giao diện người dùng), nó giúp bạn dễ dàng định nghĩa đóng gói Component giống như thẻ HTML, nó giúp bạn dễ dàng tái sử dụng khi mà dữ liệu thay đổi theo thời gian.
Không chỉ dành cho việc phát triển web, React còn dành cho việc phát triển ứng dụng mobile, desktop, ứng dụng window.
Vậy để bắt đầu với React, bạn nên bắt đầu từ đâu, và như thế nào.

Trong bài viết này, mình sẽ liệt kê những kiến thức theo thứ tự, và một số link bài viết để các bạn tham khảo. Ngoài ra mình có thể tự tìm kiếm theo từ khóa mà mình suggest để đọc thêm nhiều bài hơn.

Và xin lưu ý là không có gì bằng tài liệu chính chủ của facebook, nên nếu gặp từ khóa nào, thì nên vào trang chính của facebook nhé:  https://facebook.github.io/react/docs/

## 1. React installation
Phải nói nếu bạn là người code jquery, hay sử dụng các javascript framework thì khi chuyển sang React bạn phải gặp nhiều khái niệm gây cho bạn hoang mang tột độ.

Các kiến thức cần biết khi học React:
- ECMAScript 6 (ES6) : là 1 chuẩn mới của javascript, hỗ trợ nhiều hàm, các cú pháp viết tắt làm việc với mảng và object hiệu quả hơn.
- Babel: ES6 là 1 chuẩn mới cho nên 1 số trình duyệt sẽ chưa hỗ trợ, nên babel sẽ `transpile` ES6 -> ES5(chuẩn hiện tại mà các trình duyệt đều đọc được).
- Webpack: là một module bundler ( đóng gói các module ), hỗ trợ gói nhiều modules thành một, hoặc tách module ra thành nhiều phần để có thể tăng hiệu suất tải trang. Mặt khác webpack có rất nhiều plugin cho phép bạn có thể biên dịch less, sass, postcss gôm chung vào 1 file.
- NPM (Node package manager): là trình quản lý các gói cài đặt trong app của bạn, khi viết react app bạn sẽ có nhiều component cài đặt do người khác chia sẻ. Sử dụng cái này thì cũng đơn giản thôi.

Bạn thấy khá nhiều kiến thức đấy, nhưng đừng lo, bạn chỉ cần biết bất nhiêu là đủ, chúng ta sẽ hiểu sâu qua các bài viết thực hành.

Trước đây ở những phiên bản đầu tiên, để cài đặt 1 app React thì khá phức tạp với các bạn beginner, đôi khi cài không được sẽ khiến các bạn chán nản. 

Tuy nhiên facebook nó cho ra mắt 1 package tên là *create-react-app*, nó giúp bạn tạo 1 ứng dụng React trong vòng 1 nốt nhạc

1. Cài đặt ứng dụng đầu tiên với create-react-app: https://medium.com/@diamondgfx/learning-react-with-create-react-app-part-1-a12e1833fdc?source=user_profile---------8----------
Đây là 1 trong những bài viết sẽ giúp bạn đầu dễ dàng với 1 ứng dụng React, nó sẽ trình bài cho bạn cấu trúc cơ bản của 1 app React như thế nào, khởi tạo 1 component đầu tiên.

2. Cài đặt, cấu hình các plugin cho creact-react-app:
  https://auth0.com/blog/how-to-configure-create-react-app/
  Với các bạn mới bắt đầu mình không khuyên đọc bài viết này ^_^. Để dành sau khi các bạn đã vững về state & props.

3. Giới thiệu về cú pháp JSX
https://facebook.github.io/react/docs/introducing-jsx.html

4. Awesome React:
https://github.com/enaqx/awesome-react
Tổng hợp những bài viết hay về React, những components.

## 2. CodeEditor for development React
React sử dụng cú pháp JSX, vì vậy khi bạn sử dụng các editor thì cần phải cài thêm các gói syntax highlighter, mình xin liệt kê 1 số editor hoặc IDE code react tốt nhất hiện nay
- Webstorm: đây là 1 IDE, support đầy đủ các cú pháp mới của javascript (ES6, ES7, TypeScript, Flow, ...), gợi ý code tốt, nhắc nhở lập trình viên nếu sử dụng biến vô tội vạ :v. Đây là lựa chọn số 1, mình khuyên các bạn nên chọn nó để phát triển ứng dụng React.
- SublimeText: đây là 1 cái tên quá quen thuộc, ưu điểm nhanh gọn lẹ, nhiều plugins, nhược điểm là suggestion chưa tốt.
- Atom: tương tự như sublimetext, nhược điểm khởi động lần đâu lâu
- Nuclie: đây là 1 plguin của Atom 
- Visual Studio Code: Open Source tool từ Microsoft

## 3. Learning ES6
Với sự ra đời của ES6, thừa hưởng các cú pháp từ python, ruby, java, javascript trở nên linh bởi tính linh hoạt, cú pháp ngắn gọn dễ hiểu, nên hầu như đều được áp dụng trong mọi ứng dụng bằng Javascript hiện nay trong: Nodejs , web app, ...
Để nói về ES6 thì có rất nhiều, nhưng mình xin nói về một số tính năng đặc biết hay sử dụng nhiều nhất:
- Arrow functions
- Scoping
- String Template 
- Promise - giảm thiểu callback
- Extended Parameter Handling - Default parameter function
- Destructuring Assignment - Phân tách phần tử
- Modules - import, export - đây là một phần rất quan trọng, nó giống như namespace trong php, hay package trong java, hay python.
- Classes: Kiểu giống như hướng đối tượng như các ngôn ngữ khác
- Array: Làm việc với kiểu lists (filter, map, foreach, ...) đây là 1 phần cực kỳ quan trọng, bởi vì bạn sẽ làm việc với lists khá nhiều, bạn sẽ thấy hầu như trong các tutorial nào cũng sử dụng nó. Đọc tại MDN là chắc cú nhất: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array

Những cái features mình nói trên đều có tại link dưới đây các bạn tham khảo nhé:
- New Features: Overview & Comparison: http://es6-features.org/ 
- ES6 feautures: https://github.com/lukehoban/es6features

Và mình khuyên bạn chỉ nên đọc những cái feauture mình giới thiệu trên, rồi bắt đầu ngay vào code React luôn, khi nào gặp những cái không biêt thì search :3, chứ đọc hết có mà tẩu hỏa nhập ma.

Books
1. Understanding ES6 
https://leanpub.com/understandinges6/read
Cuốn này rất nổi tiếng, tổng hợp hầu như tất cả cấc tính năng của ES6, mình chỉ xem cuốn này như là từ điển thôi, chứ chưa đọc hết :))
2. Awesome ES6
https://github.com/ericdouglas/ES6-Learning
Cái này tổng hợp lại các bài viết nói về ES6, bao gồm các khóa học, tutorial, video ... Nói chung là nên ghé vào đây một lần cho biết ^_^

## 4. React Component, State & Props
Trong React, các thành phần đều được định nghĩa là Component, các component có thể là:
- Button
- Select
- InputText
- Textarea
- Comment (có thể chứa nhiều các component khác)
Nó được sử dụng giống như thẻ HTML, điều đó thật là tiện. Ví dụ:
```javascript
<Comment user="thanhtungdp"/>
```
Mỗi component sẽ có state & props, đây là 2 khái niệm quan trọng trong React. Hiểu được nó nội công thâm hậu, dương khí đầy mình, code như không code :))
- State: là data nội tại của component đó, state có thể khởi tạo, cập nhật thay đổi, mỗi khi thay đổi component sẽ tự động cập nhật hiển thị
- Props: là các tham số truyền vào component, props chỉ có thể đọc không thay đổi được. Như ví dụ trên kia thì props là user="thanhtungdp". Nhiệm vụ của bạn là đọc các attribute và xử lý nó hiển thị.
- Nested Component: các component lồng nhau, state của component này sẽ là props của component kia. Và dữ liệu ban đầu sẽ được lưu ở state của Root Component đầu tiên

Lý thuyết như vậy là đủ rồi, bạn nên đọc thêm các bài viết dưới đây:
1. State & props (create-react-app part 2): 
https://medium.com/@diamondgfx/learning-react-with-create-react-app-part-2-3ad99f38b48d#.zg14umu1a
Tiếp tục series bài viết create-react-app phía trên, trong bài viết này sẽ giới thiệu về cách sử dụng state và props như thế nào

2. Project HelloList với state & props (create-react-app part 3):
https://medium.com/@diamondgfx/learning-react-with-create-react-app-part-3-322447d14192#.asuk1kq0k

3. Project ShoppingList (Thinking in React by facebook):
https://facebook.github.io/react/docs/thinking-in-react.html
Bài này nằm trong loạt bài hướng dẫn cho người mới bắt đầu, bạn nên thực hành để làm quen với các cú pháp của nó

4. Project TodoLists:
https://scotch.io/tutorials/create-a-simple-to-do-app-with-react

4. Đọc thêm từ về state & props từ giác giả khác:
http://lucybain.com/blog/2016/react-state-vs-pros/
Nếu chưa hiểu mấy bài viết trên thì đọc tiếp bài này, bài này khá trong sạch và dễ hiểu

4. Đọc thêm về state & props từ trang react của facebook:
https://facebook.github.io/react/docs/components-and-props.html
https://facebook.github.io/react/docs/state-and-lifecycle.html  

5. Làm việc với form:
https://facebook.github.io/react/docs/forms.html

5. Đọc thêm các thư viện làm việc với state trong React:
https://medium.com/pro-react/a-brief-talk-about-immutability-and-react-s-helpers-70919ab8ae7c#.v28hrfh1k

## 5. React Component Life Cycle
Tạm hiểu là "Vòng đời của React Component", nó cũng giống như chu trình sinh ra và phát triển của một con người, hiểu về life cycle thì đi mây về gió, uyển chuyển như giọt nước mùa thu :)). 
Các vòng đời của nó:
- componentWillMount(): giai đoạn chuẩn bị render component lần đầu, chỉ sử dụng lần đầu tiên. Tạm hiểu đây là quá trình con đạp bụng mẹ, mẹ chuẩn bị sinh ra con ^_^
- componentDidMount(): giai đoạn sau khi render ra component lần đầu. Tạm hiểu là giai đoạn sau khi sinh con.
- componentDidUpdate(): giai đoạn component cập nhật lại khi có sự thay đổi của state và props.
- componentWillReceiveProps: giai đoạn nhận props

Ví dụ ở component là `ChatContainer` mình có khởi tạo socket, nhưng khi user chuyển sang sử dụng component khác và `ChatContainer` không còn hiển thị trên trang nữa, tuy nhiên socket vẫn còn connect, như vậy thì tốn dung lượng quá. Vì vậy cho nên mình sẽ can thiện vào vòng đời componentWillUnmount() của `ChatContainer` để close socket khi component đó không còn hiển thị trên trang.

Như mình giới thiệu các vòng đời ở trên, thì mỗi vòng đời tùy theo mục đích sử dụng, mà các bạn sẽ xử lý ở giai đoạn phụ hợp.  Nếu bạn mới bắt đầu thì bạn cũng chưa sử dụng nó nhiều đâu, hiểu là được rồi

Dưới đây mình xin liệt kê 1 số bài viết nói về nó.
- React Component lifecycle:
https://medium.com/react-ecosystem/react-components-lifecycle-ce09239010df#.uf1dhwxfp
Bài viết này khá chi tiết dễ hiểu

## 6. React router
Nếu bạn sử dụng 1 số trang web hiện nay, bạn sẽ thấy khi click vào 1 link nào đó, thì url change, nhưng trang sẽ không load lại hết thì đó là 1 ứng dụng SPA (Single page application).
Vậy làm thế nào để làm điều đó trên React, xin giới thiệu với các bạn đó là React Router.
React router khá dễ sử dụng, tài liệu chi tiết dễ hiểu.

Mình xin liệt kê một số bài viết sử dụng react router:
- Basic react router:
https://css-tricks.com/learning-react-router/
Bài này của csstricks :)) không liên quan gì tới domain nhưng mà bài viết này rất hay có hình minh họa các kiểu, nhìn rất thích
- Document:
https://github.com/ReactTraining/react-router


## 7. Fetch Data
Fetch data là 1 phần cực kỳ quan trọng trong 1 ứng dụng của bạn, nó sẽ giúp bạn tương tác với server như: post, put, delete.
Vậy làm việc với fetch data như thế nào, mình xin liệt kê 1 số bài viết

Một số thư viện cho việc fetch data:
- axios: cái này ngon lành, support server rendering (được cộng đồng sử dụng nhiều, nên dùng)
- qwest: tương tự axios, không support server rendering
- fetch: cái này thì mặc định của ES6 có support

Bài viết:
1. Ajax in React
https://daveceddia.com/ajax-requests-in-react/
Bài này là bài cơ bản

2.  Working with server;
https://www.fullstackreact.com/articles/using-create-react-app-with-a-server/
Nâng cao hơn 1 tí ^_^

3. How ajax work reacts
http://andrewhfarmer.com/how-ajax-works-react/

3. React Ajax best practices
http://andrewhfarmer.com/react-ajax-best-practices/

4. Container components:
https://css-tricks.com/learning-react-container-components/
Bài này của rất hay, các bạn nên đọc nhé.


## 8. Redux - Store management
Một phần khá quan trọng trong React đó chính là việc quản lý Store. 
Nếu bạn không áp dụng 1 lib store management nào, thì công việc bạn cần làm đó chính là pass props liên vào các component con. Hãy nghĩ tới việc bạn có 10 cái nested component, và bạn phải truyền data từ root component tới component thứ 10 để đọc dữ liệu, đó là 1 điều thật kinh khủng :3
Redux sẽ giúp bạn giải quyết vấn đề đó, làm cho ứng dụng của bạn trở nên logic, dễ dàng quản lý hơn.

Bài viết:
- Basic redux: 
https://css-tricks.com/learning-react-redux/
Bài này rất hay của bác csstricks, theo mình là dễ hiểu nhất từ trước tới giờ mình đọc
- Learn redux with cartoon:
https://code-cartoons.com/a-cartoon-intro-to-redux-3afb775501a6#.8wb7q2mie
Mô tả bằng các hình ảnh hoạt hình vui nhộn
- Getting started with redux video: https://egghead.io/courses/getting-started-with-redux
- Fullstack redux:
 https://teropa.info/blog/2015/09/10/full-stack-redux-tutorial.html
Bài này từ năm 2015 nhưng rất hay và chi tiết, nếu có thời gian và muốn nâng cao sâu trình độ thì đọc, còn nếu không thì đọc sơ qua thôi :v
- Awesome redux:
 https://github.com/xgrommx/awesome-redux
Các bạn đọc thêm 1 số project ở trang này nhé, nhiều lắm tha hồ mà đọc :v
- Smart & dumb component:
http://jaketrent.com/post/smart-dumb-components-react/
Redux hoạt động theo cơ chế này đọc để hiểu thêm.
- Series bài viết build 1 blog với redux:
 https://medium.com/@rajaraodv/a-guide-for-building-a-react-redux-crud-app-7fe0b8943d0f#.1f7nnie6n
 
Tóm lại thì redux rất nhiều bài viết, mình chỉ giới thiệu cơ bản thôi, các bạn nên tìm trong phần awesome redux nhé

## 9. Medium chanel
Mình xin giới thiệu các bạn 1 số chanel trên medium nói về việc phát triển ứng dụng với React, React Native và 1 số kiến thức về phát triển hệ thống mà hi
- https://medium.mybridge.co: Kiến thức quá nhiều, đưng lo trang này sẽ tổng hợp giúp bạn những bài viết nổi bật theo tháng. Dưới đây là 1 ví dụ, các bạn chỉ cần vào trang và search từ khóa reactjs
	- Top 10 reacjts articles last month may: https://medium.mybridge.co/top-10-react-js-articles-from-last-month-v-may-ceb5420b91df#.nqrnux5yt
- https://medium.freecodecamp.com/: Cái này thì trùm rồi, vào search từ khóa reactjs là ra cả đống bài.
- https://hackernoon.com/: tương tự như freecodecamp
- https://code-cartoons.com/ Cái bài viết ở đây đều rất vui nhộn, nó có những hình ảnh minh họa làm cho bạn dễ hiểu, làm kích thích học reactjs hơn ^_^
- https://medium.com/walmartlabs: Walmart là hệ thống bán lẻ hàng đầu ở mỹ, hãy xem các kỹ sư chia sẻ về xây dựng kiến trúc hệ thống.
- https://medium.com/@ReactJS_News: Cập nhật tin tức về React
- https://medium.com/@_ericelliott: Bác này trùm về javascript, tác giả của understanding javascript ES6
- https://medium.com/airbnb-engineering: Airbnb sử dụng React hầu như trong hệ thống của họ, xem những bài chia sẻ của họ để hiểu thêm.
- http://www.wix.engineering Wix là 1 trong những website cung cấp nền tảng CMS phổ biến nhất hiện nay, nghe các bác kỹ sư chia sẻ và chém gió
- https://medium.com/react-native-training: Kênh training react native có khá nhiều bài viết hay về nó
- https://dev-blog.apollodata.com/

Một số kênh khác mình hay theo dõi để trau dồi kiến thức design, tăng cao ý tưởng :3:
- https://blog.prototypr.io/
- https://uxplanet.org/
- https://medium.muz.li/
- https://medium.com/ux-power-tools

## 10. Bonus posts
- 22 Amazing open source React projects:
https://medium.mybridge.co/22-amazing-open-source-react-projects-cb8230ec719f#.c3pdfmttu
- Learn How to Create Quick and Simple React Flipping Card
https://medium.com/@AlexDevero/learn-how-to-create-quick-and-simple-react-flipping-card-7b4660bca475#.1427sr5ll
- How I converted my React app to VanillaJS (and whether or not it was a terrible idea)
https://hackernoon.com/how-i-converted-my-react-app-to-vanillajs-and-whether-or-not-it-was-a-terrible-idea-4b14b1b2faff#.nv1cik6vc
- GraphQL explained
https://dev-blog.apollodata.com/graphql-explained-5844742f195e#.y1rnwdop4
- 230 Curated Resources and Tools for Building Apps with React.js
https://appendto.com/2016/12/230-resources-and-tools-for-building-apps-with-react-js/
- Bài viết học React Native của mình:
https://www.facebook.com/notes/react-vi%E1%BB%87t-nam/react-native-nh%E1%BB%AFng-b%C3%A0i-vi%E1%BA%BFt-step-by-step-d%C3%A0nh-cho-c%C3%A1c-b%E1%BA%A1n-m%E1%BB%9Bi-h%E1%BB%8Dc/1772834179637935?__mref=message_bubble

## 11. Real Projects
- Build A Media Library with React, Redux, and Redux-saga:
https://scotch.io/tutorials/build-a-media-library-with-react-redux-and-redux-saga-part-1
- Build Bookshop with react & redux:
https://scotch.io/tutorials/build-a-bookshop-with-react-redux-i-react-redux-flow
- Clone Yelp:
https://www.fullstackreact.com/articles/react-tutorial-cloning-yelp/
- JWT authentication with react redux:
http://www.thegreatcodeadventure.com/jwt-authentication-with-react-redux/
- Soundclound app:
https://www.robinwieruch.de/the-soundcloud-client-in-react-redux/
- Build blog management with redux:
 http://blog.isquaredsoftware.com/2016/10/practical-redux-part-0-introduction/
Bài viết này khá hay và chi tiết, có hình ảnh minh họa, chia theo series nên rất dễ theo dõi và nắm bắt
- Clone instagram app:
http://www.eloquentwebapp.com/instagram-app-node-react-redux/
- Build app cabin:
http://cabin.getstream.io/
"Cabin is built using React and Redux. Stream powers the feed technology, Algolia search, Mapbox the custom maps, Keen analytics and ImgIX the image resizing. These APIs are powerful and scalable and allow you to build a fully featured app."
Series bài viết này hướng dẫn các bạn sử dụng React với các dịch vụ thứ 3
- Build app trello clone:
https://blog.diacode.com/trello-clone-with-phoenix-and-react-pt-1
- Creating a Cordova Hybrid App with React, Redux and Webpack
https://onsen.io/blog/cordova-hybrid-app-with-react-redux-webpack/
- Build a Music Streaming App with Electron, React & ES6
https://www.sitepoint.com/music-streaming-app-electron-react-es6/

Bấy nhiêu thôi, mình research cũng đuối quá, anh em vào trang mybridge medium để search thêm nhé, nhiều lắm ^_^, mình tổng hợp 1 số cái nổi bật

## 12. Books
- Pro React:  Cuốn này các bạn nên đọc, hiện tại đã cập nhật sử dụng Redux. Nhờ cuốn này mà kiến thức về React của mình vững, làm nền tảng để học mấy cái khác.
Pro react sẽ hướng dẫn bạn từng bước từng bước xây dựng ứng dụng React từ thuần Component cho tới kiến trúc Flux, nó giới thiệu và áp dụng các thư viện helpers của react như: update-addons, transitions, react-router, react-dnd(drag and drop).
Kết quả sau khi đọc sau cuốn sách này:
	- Nắm bắt được các kiến thức về React Component, Async
	- Hiểu được Immutable, Mutable là gì :v
	- Nắm bắt được kiến trúc Flux, là cơ sở để triển khai sang Redux
	- Sử dụng thành thạo các thư viện của React
	- Isomorphic React Applications - cái này hiểu là ứng dụng ` đồng hình`, tức là nó sẽ render ra dữ liệu phía server luôn.
	- Unit test
	- Và cuối cùng bạn sẽ có một ứng dụng quản lý task chuyên nghiệp (kéo thả các kiểu y như trello :v)
- survivejs.com: Mình có đọc qua các bài viết trên này, thấy đây là 1 trang khá hay cung cấp mấy cái project thực hành khá là trực quan.
- fullstackreact.com: Trang này tương tự như survivejs, cái nào cũng hay cả.
- ReactJS by example:
http://reactkungfu.com/react-by-example/
Cung cấp các ví dụ về component react, bạn nào mới bắt đầu thì nên tìm cuốn này đọc thêm

Cũng có vài cuốn khác nhưng mà mình chưa đọc, mình chỉ đọc mấy cuốn trên và đưa ra nhận xét.

Còn rất nhiều bài viết hay khác về React, các bạn chỉ cần follow theo mấy cái link mình đưa thì sẽ ra rất nhiều bài viết về react.

Chúc các bạn học react vui vẻ ^_^

