# 1. Mở đầu: Chatbot là gì?

Hẳn bạn đã từng nhắn tin hỏi thông tin trên website một công ty nào đó, và ngay lập tức nhận được câu trả lời như thể đang chat với một nhân viên tư vấn thật sự. Hoặc đơn giản hơn, bạn đã thử hỏi Siri "Hôm nay thời tiết thế nào?" hay nhờ Google Assistant đặt báo thức. Đó chính là chatbot - một chương trình máy tính được thiết kế để trò chuyện với con người thông qua văn bản hoặc giọng nói, gần giống như cách bạn trò chuyện với một người thật.

Nghe có vẻ đơn giản phải không? Nhưng thật sự chatbot ngày nay đã tiến hóa vượt xa những "chatbot cổ điển" mà bạn có thể từng gặp cách đây vài năm. Những chatbot ngày xưa chỉ có thể trả lời theo những kịch bản có sẵn, giống như một menu lựa chọn cứng nhắc: "Nhấn 1 để hỏi về giá", "Nhấn 2 để hỏi về địa chỉ"... Còn chatbot hiện đại? Chúng có thể hiểu ngữ cảnh, ghi nhớ cuộc hội thoại, thậm chí "sáng tạo" ra câu trả lời chưa từng được lập trình sẵn.

## 1.1. Bài viết này sẽ giúp bạn hiểu gì?
Trong bài viết này, chúng tôi sẽ đưa bạn đi từ những khái niệm cơ bản nhất về chatbot, cho đến việc giải mã cách hoạt động của các AI chatbot hiện đại - những "siêu trí tuệ nhân tạo" như ChatGPT, Google Bard hay Claude. Đặc biệt, chúng ta sẽ tập trung vào các chatbot được xây dựng dựa trên Large Language Models (LLM) - những mô hình ngôn ngữ lớn đang làm thay đổi cách chúng ta tương tác với máy móc.

## 1.2. Hãy cùng phân biệt hai "thế hệ" chatbot:
<p align="center">
  <img src="https://aioconquer.aivietnam.edu.vn/static/uploads/20260116_095833_3e05dc57.png" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 1.1. Hai thế hệ chatbot</em>
</p>

### a. Rule-based Chatbot (Chatbot dựa trên quy tắc)

- Hoạt động theo kịch bản được lập trình sẵn
- Giống như một cây quyết định: "Nếu người dùng nói A thì trả lời B"
- Ưu điểm: Dễ kiểm soát, chính xác trong phạm vi hẹp
- Nhược điểm: Không linh hoạt, không hiểu câu hỏi ngoài kịch bản

### b. AI-powered Chatbot (Chatbot dựa trên AI)

- Sử dụng Machine Learning và Deep Learning để "học" cách trả lời
- Có khả năng hiểu ngữ cảnh, xử lý ngôn ngữ tự nhiên phức tạp
- Ưu điểm: Linh hoạt, có thể xử lý vô số tình huống khác nhau
- Nhược điểm: Phức tạp hơn, đôi khi khó dự đoán

Và đây là điều thú vị: Chatbot AI hiện đại không chỉ "thông minh" hơn về mặt kỹ thuật, mà còn mang lại trải nghiệm gần gũi và tự nhiên hơn rất nhiều so với những người tiền nhiệm của chúng. Vậy bí mật đằng sau sự tiến hóa này là gì? Chúng ta sẽ cùng khám phá!

# 2. Vì sao chúng ta cần AI chatbot?

Trước khi đi sâu vào "bên trong" một chatbot hoạt động như thế nào, có lẽ bạn đang tự hỏi: "Tại sao chúng ta lại cần đến AI chatbot? Chatbot đơn giản theo quy tắc không đủ sao?"
Câu trả lời nằm ở ba yếu tố quan trọng: Quy mô, Tốc độ, và Trải nghiệm người dùng.

## 2.1. Quy mô: Phục vụ hàng triệu người cùng lúc
Hãy tưởng tượng bạn là chủ của một công ty thương mại điện tử lớn. Mỗi ngày có hàng chục nghìn khách hàng truy cập website và đặt câu hỏi: "Đơn hàng của tôi đến khi nào?", "Sản phẩm này có màu xanh không?", "Làm sao để đổi trả hàng?"...
Với chatbot rule-based truyền thống, bạn sẽ phải:

- Lập trình từng kịch bản cho từng loại câu hỏi
- Liên tục cập nhật khi có sản phẩm mới, chính sách mới
- Vẫn không thể xử lý các câu hỏi "ngoài kịch bản"

Nhưng với AI chatbot, hệ thống có thể:

- Tự động hiểu ngữ cảnh và ý định của khách hàng
- Trả lời hàng triệu câu hỏi khác nhau mà không cần lập trình riêng
- Học hỏi từ mỗi cuộc hội thoại để cải thiện theo thời gian

## 2.2 Tốc độ: Phản hồi tức thì, 24/7
Trong thời đại số, không ai muốn chờ đợi. Một nghiên cứu của HubSpot cho thấy 90% khách hàng mong đợi phản hồi tức thì khi họ có câu hỏi dịch vụ khách hàng. AI chatbot có thể:

- **Trả lời ngay lập tức:** Không cần thời gian chờ đợi như khi liên hệ với tổng đài
- **Hoạt động 24/7:** Không giới hạn giờ làm việc, múi giờ hay ngày nghỉ lễ
- **Xử lý đồng thời:** Một chatbot có thể "nói chuyện" với hàng nghìn người cùng lúc

Điều này không chỉ cải thiện trải nghiệm khách hàng mà còn giúp doanh nghiệp tiết kiệm chi phí vận hành đáng kể.
## 2.3. Trải nghiệm người dùng: Giao tiếp tự nhiên như con người
Đây chính là điểm mạnh nhất của AI chatbot so với các thế hệ trước. Thay vì phải nhớ các từ khóa cụ thể hoặc chọn từ menu cứng nhắc, người dùng có thể:

**Nói chuyện tự nhiên:**

- ❌ Chatbot truyền thống: "Bạn muốn kiểm tra đơn hàng? Vui lòng nhập mã đơn hàng."
- ✅ AI chatbot: "Chào bạn! Mình thấy bạn có đơn hàng #12345 đang trên đường giao. Bạn muốn biết thêm thông tin gì không?"

**Hiểu ngữ cảnh:**

- Người dùng: "Tôi muốn mua một chiếc điện thoại"
- Chatbot: "Bạn có ngân sách dự kiến bao nhiêu?"
- Người dùng: "Khoảng 10 triệu"
- Chatbot: "Vậy mình recommend cho bạn các mẫu sau..." *(chatbot nhớ được ngữ cảnh "điện thoại" và "10 triệu")*

**Cá nhân hóa:**
AI chatbot có thể phân tích lịch sử tương tác, sở thích của người dùng để đưa ra gợi ý phù hợp hơn, tạo cảm giác như đang được phục vụ bởi một trợ lý cá nhân.

## 2.4. Các ứng dụng thực tế
AI chatbot đã và đang xuất hiện ở khắp mọi nơi:
<p align="center">
  <img src="images\chatbot_usecase_mindmap.png" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 2.1. Các ứng dụng thực tế của AI chatbot</em>
</p>

**Dịch vụ khách hàng:**

- Ngân hàng: Kiểm tra số dư, lịch sử giao dịch, chặn thẻ
- Bảo hiểm: Tra cứu hợp đồng, hướng dẫn bồi thường
- Bán lẻ: Tư vấn sản phẩm, theo dõi đơn hàng

**Giáo dục:**

- Trợ giảng ảo: Trả lời thắc mắc của sinh viên
- Học ngoại ngữ: Luyện tập hội thoại tiếng Anh, Trung, Nhật...

**Y tế:**

- Tư vấn sơ bộ: Triệu chứng bệnh, lịch khám
- Nhắc nhở uống thuốc, chăm sóc sức khỏe

**Giải trí & Trợ lý cá nhân:**

- ChatGPT, Claude: Trợ lý viết lách, lập trình, brainstorming ý tưởng
- Siri, Google Assistant: Điều khiển thiết bị thông minh, đặt lịch hẹn

# 3. Quy trình một lượt chat diễn ra như thế nào?

Bạn từng tự hỏi: Từ lúc bạn nhấn Enter đến khi chatbot trả lời chỉ tốn vài giây, điều gì đã xảy ra?

**Cơ chế hoạt động của AI chatbot (NLP)**<br/>
Cách hoạt động của các chatbot sử dụng NLP (Natural Language Processing) thực chất bao gồm một chuỗi các bước khá logic để hiểu và trả lời người dùng một cách tự nhiên. Mình giải thích ngắn gọn, đơn giản như sau:

<p align="center">
  <img src="images/AI_chatbot_WorkFlow.svg" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 3.1. Quy trình xử lý một lượt chat của AI chatbot sử dụng NLP</em>
</p>

**1. Xử lý đầu vào** (Input Processing)

Khi bạn gửi tin nhắn, chatbot sẽ phân tích đoạn văn: tách thành từng từ (tokenization), xác định loại từ (danh từ, động từ…), và nhận diện các thông tin quan trọng như tên người, ngày tháng, địa điểm… Nói đơn giản là bước “đọc và hiểu sơ bộ” nội dung bạn vừa nhập.
<p align="center">
  <img src="images\input_processing.png" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 3.2. Xử lý đầu vào (Input Processing)</em>
</p>

**2. Nhận diện ý định (Intent Recognition)**

Sau khi phân tích, chatbot xác định mục đích chính của bạn: bạn đang hỏi thông tin, yêu cầu làm gì đó, phản hồi, hay chỉ trò chuyện thôi? Bước này thường dùng mô hình phân loại để gán một nhãn ý định (intent). Nhờ vậy bot biết nên tra dữ liệu, gọi API, hay sinh câu trả lời tự nhiên.
<p align="center">
  <img src="images\intent_recognition.png" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 3.3. Nhận diện ý định (Intent Recognition)</em>
</p>

**3. Quản lý hội thoại (Dialogue Management)**

Ở bước này, hệ thống quyết định “mạch" hội thoại:

- Dùng ngữ cảnh trước đó (những gì đã nói trong cuộc chat) để giữ câu trả lời liên tục, hợp lý.
- Chọn hành động tiếp theo: trả lời trực tiếp, gọi API (ví dụ tra lịch bay), cập nhật trạng thái, hay hỏi - thêm.
- Hệ thống quản lý giống như người điều phối cuộc trò chuyện để không bị lạc đề hoặc quên thông tin quan trọng.

**4. Tạo câu trả lời (Response Generation)**

Dựa trên ý định và ngữ cảnh, bot sẽ:<br/>
- Tìm thông tin từ cơ sở dữ liệu
- Thực hiện một hành động nào đó (như tra cứu, đặt lệnh)
- Hoặc tự tạo câu trả lời tự nhiên bằng các kỹ thuật sinh ngôn ngữ (natural language generation).
<p align="center">
  <img src="images\dialogue_management.png" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 3.4. Quản lý hội thoại và sinh câu trả lời</em>
</p>

**5. Học hỏi và cải thiện**

Không chỉ trả lời rồi thôi, chatbot còn có khả năng học từ các cuộc trò chuyện trước đó.
Thông qua dữ liệu tương tác, phản hồi của người dùng và các lần sửa lỗi, hệ thống dần cải thiện khả năng hiểu ngôn ngữ, nhận diện ý định chính xác hơn và đưa ra câu trả lời phù hợp hơn theo thời gian.

Nhờ cơ chế này, chatbot càng được sử dụng nhiều thì càng “thông minh” và linh hoạt hơn.
<p align="center">
  <img src="images\feedback.png" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 3.5. Chatbot học hỏi và tối ưu dựa trên phản hồi người dùng</em>
</p>

**6. Trả lời người dùng**

Cuối cùng, bot gửi lại câu trả lời dưới dạng văn bản (hoặc giọng nói), sao cho dễ đọc và thân thiện nhất có thể.
<p align="center">
  <img src="images\chat-ui.gif" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 3.6. Chatbot phản hồi sao cho dễ đọc và thân thiện nhất với người dùng</em>
</p>

*Quy trình này nghe có vẻ dài dòng nhưng thực tế nó diễn ra chỉ trong vài giây. Tất cả đều được xử lý tự động để mang lại cho bạn cảm giác như đang trò chuyện với một người bạn thực sự chứ không phải một cỗ máy vô tri.*

# 4. Main technologies in AI chatbot

Unlike their rule-based counterparts, AI chatbots use advanced technologies in AI to not only optimize its accuracy but also how natural it sounds when answering user questions. It also enables the chatbots to respond based on different context.

**4.1. NLP - Natural Language Processing:**

Natural Language Processing (NLP) allows AI systems to identify language and characters and to interpret grammar, context in text, speech, or conversations. By applying NLP, chatbots can effectively provide natural and comprehensively responses based on user’s context, unlocking more general and accurate information to user.

Key technologies of NLP using in AI chatbots:
Tokenization: Break down raw text into smaller units, which can be words, subwords, characters, or sentences, to make unstructured text understandable for machines. It helps to the keywords to process, analyze and understand human language to respond appropriately.
Example: "Book a flight tomorrow" → ["Book", "a", "flight", "tomorrow"]

<p align="center">
  <img src="images\part4_tokenization.png" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 4.1. Tokenization</em>
</p>

- Named Entity Recognition — NER: Recognize words, subwords in context and classifies them into groups such as human name, organization, location, time, product to help chatbots respond based on these entities.
Example: "What's the weather in Chicago tomorrow?" → Chicago is the entity to describe the location for chatbots to answer question about weather.

<p align="center">
  <img src="images\part4_NER.png" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 4.2. NER - Named Entity Recognition</em>
</p>

- Sentiment analysis: Identify and quantify opinions, emotions, and attitudes in text, speech, classifying them as positive, negative, or neutral to understand subjective information. It helps chatbots respond with a more pleasing, emotional tone to users.

<p align="center">
  <img src="images\part4_sentiment_analysis.png" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 4.3. Sentiment Analysis</em>
</p>

**4.2. AI models / Machine Learning / LLM:**

These technologies are the brain of AI chatbot, the data is trained, reinforced to help optimize the chatbot responses.

Machine Learning: Machine Learning algorithms helps train the chatbot how to process and respond to user based on predefined data.

Deep Learning: Allow chatbots to continuously learn from interactions, improving their ability to handle complex conversations

Large Language Models (LLMs): are trained on massive amounts of linguistic data, including grammar, spelling, and multiple languages. These models are used in chatbot training as a core approach to enable chatbots to accurately analyze user conversations and generate more natural and human-like responses.

<p align="center">
  <img src="images\part4_ML_DL_LLM_GenAI.png" style="margin: 0 auto; display: block;"><br/>
  <em>Hình 4.4. Technologies uses to train AI chatbot</em>
</p>

In addition to the technologies mentioned above, Generative AI is now being used in chatbot training to improve performance. Generative AI turns chatbots from basic question-and-answer tools into AI agents, making conversations feel more like real human consultations. Instead of giving fixed or repetitive answers, chatbots can provide more flexible responses and reason to offer suggestions beyond their training data, while still staying relevant to the context of the conversation.

**4.3. Feedback and Continuous Learning:**

In addition to answering user questions, AI chatbots can continue learning based on users’ current responses. Data is continuously updated from ongoing conversations with both the current user and other users on the same topics, allowing the chatbot to optimize and expand its knowledge. As a result, the chatbot becomes smarter over time.

# 5. Các ví dụ so sánh 

## 5.1. Chatbot và trợ lý con người: giống và khác nhau ở đâu?

Hãy tưởng tượng bạn bước vào một cửa hàng điện thoại và hỏi:

*“Điện thoại này pin dùng được có lâu không?”*

Một trợ lý con người sẽ:

* Nghe câu hỏi

* Hiểu bạn là người quan tâm về pin "nguồn sống của một chiếc điện thoại"

* Dựa vào kinh nghiệm thực tế và ngữ cảnh để tư vấn

* Có thể hỏi thêm để làm rõ nhu cầu của bạn

Trong khi đó, AI chatbot xử lý câu hỏi theo cách khác:

* Nó không “nghe”, mà đọc chữ

* Không “hiểu” theo nghĩa nhận thức, mà phân tích mẫu ngôn ngữ

* Dựa trên dữ liệu đã học để dự đoán câu trả lời phù hợp nhất

Nói cách khác, chatbot hiện đại chủ yếu hoạt động bằng cách tạo phản hồi dựa trên xác suất, chứ không có khả năng hiểu hay suy luận như con người.

## 5.2. So sánh giữa các chatbot phổ biến: ChatGPT, Gemini, Copilot

 Mặc dù đều được gọi là “AI chatbot”, nhưng mỗi hệ thống **được thiết kế cho mục tiêu khác nhau**.

| **Chatbot**             | **Mục tiêu chính**           | **Thế mạnh nổi bật**                                                            | **Phù hợp khi nào**                                                                        | **Context / Text Window (khái quát)**                    | **Hạn chế kỹ thuật chính**                                               |
| ----------------------- | ---------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ | -------------------------------------------------------- | ------------------------------------------------------------------------ |
| **ChatGPT**             | Hội thoại tổng quát          | Giải thích kiến thức, trả lời câu hỏi, viết nội dung đa lĩnh vực                | Khi người dùng muốn “nói chuyện”, hỏi nhiều chủ đề khác nhau, hoặc cần giải thích dễ hiểu  | Lớn – hỗ trợ hội thoại dài, nhớ được nhiều lượt trao đổi | Có thể tạo câu trả lời sai nhưng tự tin; phụ thuộc dữ liệu huấn luyện    |
| **Gemini (Google)**     | Tra cứu & tổng hợp thông tin | Tìm kiếm, tổng hợp dữ liệu từ nhiều nguồn, tích hợp sâu với hệ sinh thái Google | Khi cần tra cứu thông tin, phân tích dữ liệu, hoặc làm việc gắn với các dịch vụ của Google | Rất lớn – tối ưu cho xử lý văn bản dài và nhiều nguồn    | Dễ cho kết quả mang tính tổng quát; phụ thuộc mạnh vào ngữ cảnh tìm kiếm |
| **Copilot (Microsoft)** | Hỗ trợ công việc             | Viết code, soạn email, làm việc với tài liệu Office                             | Khi cần một trợ lý hỗ trợ trực tiếp trong quá trình làm việc hằng ngày                     | Trung bình – lớn, tối ưu theo ngữ cảnh công việc         | Giới hạn ngoài môi trường làm việc; phụ thuộc hệ sinh thái Microsoft     |

<p align="center">  
<em>Bảng 5.1. So sánh giữa các AI chatbot</em>
</p>

Nói đơn giản:

* ChatGPT giống một người bạn biết nhiều thứ

* Gemini giống một trợ lý nghiên cứu

* Copilot giống một đồng nghiệp hỗ trợ công việc

Điểm chung là cả ba đều dựa trên **mô hình ngôn ngữ lớn** (LLM) – loại mô hình học từ lượng dữ liệu khổng lồ để sinh ra văn bản mới.

Điểm khác nhau nằm ở **cách triển khai và ngữ cảnh sử dụng**, không hẳn là “ai thông minh hơn ai”.

# 6. Những vấn đề thường gặp và giới hạn của AI chatbot 
## 6.1. Chatbot có thể hiểu nhầm nhưng trả lời rất tự tin

Một đặc điểm dễ gây hiểu lầm của AI chatbot là: **trả lời nghe rất hợp lý, nhưng vẫn có thể sai.**

Nguyên nhân là vì chatbot không kiểm chứng thông tin như con người, mà chỉ dự đoán câu trả lời có xác suất cao nhất dựa trên dữ liệu đã học. Khi gặp câu hỏi mơ hồ, thiếu ngữ cảnh, hoặc nằm ngoài phạm vi dữ liệu, chatbot vẫn có thể “đoán” và tạo ra câu trả lời nghe thuyết phục.

Đây là hạn chế cốt lõi của các mô hình ngôn ngữ: chúng xử lý ngôn ngữ dựa trên mẫu thống kê, không có hiểu biết thực sự về thế giới.

## 6.2. Chatbot không thể thay thế hoàn toàn con người

Dù rất hữu ích, AI chatbot vẫn có những giới hạn rõ ràng:

* Không có cảm xúc thật

* Không hiểu đầy đủ bối cảnh xã hội

* Không chịu trách nhiệm cho quyết định

* Trong nhiều lĩnh vực như giáo dục, y tế hay chăm sóc khách hàng, chatbot thường chỉ đóng vai trò hỗ trợ, giúp giảm tải công việc cho con người chứ không thay thế hoàn toàn.

Một kết luận cho rằng chatbot hiệu quả nhất khi được thiết kế để bổ trợ con người, chứ không phải đóng vai trò như một “con người nhân tạo”.

## 6.3. Chatbot phụ thuộc rất lớn vào dữ liệu huấn luyện


Chất lượng của AI chatbot phụ thuộc trực tiếp vào:

* Lượng dữ liệu huấn luyện

* Chất lượng dữ liệu

* Cách cập nhật và tinh chỉnh mô hình

Nếu dữ liệu không đầy đủ hoặc thiên lệch, chatbot có thể đưa ra câu trả lời sai hoặc mang định kiến. Bias trong dữ liệu là một trong những thách thức lớn nhất của NLP hiện nay.
Vì vậy, chatbot không phải là hệ thống “xong là xong”, mà cần được huấn luyện, đánh giá và cải thiện liên tục.

*Qua bài viết này, bạn đã có cái nhìn tổng quan về AI chatbot: từ khái niệm cơ bản, lý do ra đời, quy trình xử lý một lượt trò chuyện cho đến các công nghệ cốt lõi bên trong. Nhờ sự kết hợp giữa xử lý ngôn ngữ tự nhiên và các mô hình AI hiện đại như Large Language Models, chatbot bây giờ không chỉ trả lời theo kịch bản có sẵn mà còn có khả năng hiểu ngữ cảnh, tạo phản hồi linh hoạt và học hỏi dần theo thời gian. Chính vì vậy, AI chatbot đang trở thành một công cụ hữu ích trong nhiều lĩnh vực như chăm sóc khách hàng, học tập, làm việc và giải trí, giúp tiết kiệm thời gian, nâng cao trải nghiệm người dùng và mở ra nhiều tiềm năng ứng dụng trong tương lai.*

**REFERENCES**

* Brown, T. B., Mann, B., Ryder, N., Subbiah, M., Kaplan, J., Dhariwal, P., … Amodei, D. (2020). Language models are few-shot learners. Advances in Neural Information Processing Systems, 33, 1877–1901. [https://arxiv.org/abs/2005.14165](https://arxiv.org/abs/2005.14165)

* Hovy, D., & Prabhumoye, S. (2021). Five sources of bias in natural language processing. Language and Linguistics Compass, 15(8), e12432. [https://doi.org/10.1111/lnc3.12432](https://doi.org/10.1111/lnc3.12432)

* Jurafsky, D., & Martin, J. H. (2023). Speech and language processing (3rd ed., draft). Stanford University. [https://web.stanford.edu/~jurafsky/slp3/](https://web.stanford.edu/~jurafsky/slp3/)

* Shum, H.-Y., He, X., & Li, D. (2018). From Eliza to XiaoIce: Challenges and opportunities with social chatbots. arXiv. [https://arxiv.org/abs/1812.08989](https://arxiv.org/abs/1812.08989)

* Zhang, Y., Sun, S., Galley, M., Chen, Y.-C., Brockett, C., Gao, X., … Dolan, B. (2024). A complete survey on LLM-based AI chatbots. arXiv. [https://arxiv.org/abs/2406.16937](https://arxiv.org/abs/2406.16937)

* GeeksforGeeks. (n.d). What is Natural Language Processing? [https://www.geeksforgeeks.org/nlp/what-is-natural-language-processing-nlp-chatbots/](https://www.geeksforgeeks.org/nlp/what-is-natural-language-processing-nlp-chatbots/)
