title: 색 접근성: 포용적인 제품 디자인에 도움이 되는 도구와 정보
author: Stéphanie Walter
source: https://stephaniewalter.design/blog/color-accessibility-tools-resources-to-design-inclusive-products/

# 색 접근성: 포용적인 제품 디자인에 도움이 되는 도구와 정보

[기본적인 접근성과 색상에 대해 학생들에게 가르치는 것에 대한 짧은 트윗](https://twitter.com/WalterStephanie/status/1111960235491639296)을 남겼는데, 꽤 많은 관심을 받았습니다. 이로 인해 색 접근성에 대해 흥미로운 토론을 하게 되었습니다 (의도하진 않았던 이모지에 대한 토론도요 ^^). 그래서 제가 평소에 제품 제작과 검토에 사용하는 색 접근성에 대한 모든 정보와 팁, 그리고 도구들을 한 번 정리해보았습니다. 함께 보시죠.

## 대비와 접근성: 색에 대한 몇 가지 기본 사항

제품을 만들 때 (디지털에 대해 얘기하겠지만 다른 제품에도 적용 가능합니다), 색 선택은 중요합니다. 색을 통해 브랜드 정체성을 드러내며, 정보를 이해하기 쉽게 하기도 합니다. 불행하게도, **모든 사람이 같은 방식으로 색상을 경험하지는 못합니다**. 어떤 사람은 **색맹**이거나, **시각 장애**를 가지고 있을 수 있으며, 사람마다 다양한 환경에 놓여있을 것입니다. 그렇기 때문에 제품에 색을 사용할 때 **접근성에 대해 더 신경 써야 합니다**.

저는 접근성 전문가가 아니기 때문에 모든 세부사항을 다루지는 않을 겁니다. 접근성에 대해 알아야 할 것이 있다면 [WCAG 2.1 지침](https://www.w3.org/TR/WCAG21)에서 당신에게 도움이 될 기준 목록을 찾아볼 수 있습니다. 이 짧은 글에서는 **AA 기준**을 중심으로 알아볼 것입니다. HTML 표준 문서처럼 좀 두렵게 느껴질 수 있음을 이해합니다. 이 장대한 목록에서 [1.4 장](https://www.w3.org/TR/WCAG21/#use-of-color)은 “배경에서 전경을 분리하는 것을 포함해 사용자가 콘텐츠를 보고 듣기에 편하게 하는 것”을 다룹니다.

접근성과 색에 대해서라면, 이 두 가지를 반드시 기억하세요.

  1.  **색상을 정보와 행동 등을 나타내는 유일한 시각적 수단으로 사용하지 마세요**.
  1.  **배경과 전경 사이에 충분한 대비를 가지게 하세요** (전경에는 문자열과 아이콘 외에 입력 양식의 테두리와 다른 요소들도 포함됩니다).

![두 기준에 대한 시각적 설명](https://stephaniewalter.design/wp-content/uploads/2019/04/2main-coloraccessibility-rules.jpg)

첫 번째 기준은 예를 들어, 그래프를 그릴 때 서로 다른 항목을 쉽게 구분할 수 있도록 색상 외에 다른 방법을 제공해야 한다는 것입니다. [트렐로에 이에 대한 좋은 예제가 있습니다](https://wearecolorblind.com/examples/trello-colorblind-friendly-mode/). 입력 양식에 대해서도 문제점을 보여줄 때 빨간 테두리만 쳐서는 안 됩니다. [성공 기준 이해 1.4.1: 색상 사용](https://www.w3.org/WAI/WCAG21/Understanding/use-of-color.html) 페이지에서 예제를 더 찾아보세요.

두 번째 기준은 문자열(또는 전경 요소)과 (배경)색상 사이의 대비가 아래와 같아야 함을 의미합니다.

  *  **4.5 대 1** – **18포인트 이하**의 문자열과 **14포인트 이하의 굵은** 문자열
  *  **3 대 1 ** – **18포인트 이상**의 문자열과 **14포인트 이상의 굵은** 문자열

포인트에서 픽셀값으로의 변화는 간단하지는 않지만, [성공 기준 이해 1.4.3: 대비 (최소)](https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum.html)에서 자세히 알아볼 수 있습니다.

간단하게는 **24픽셀 이하의 작은 문자열** (굵은 경우 19픽셀)은 **4.5 대비 규칙을 따르고**, **24픽셀 이상의 큰 문자열** (굵은 경우 19픽셀 이상)은 **3 대비 규칙을 따르세요**.

네네, “하지만 4.5나 3의 명암비를 가지는지 어떻게 측정하나요? 각각의 색 조합에 대해 다 계산해야 하나요?!” 같이 생각할 수 있겠습니다. 걱정하지 마세요. 바로 사용할 수 있는 도구와 정보를 알려드릴게요.

## 색맹 시뮬레이션 도구

첫 번째 기준은 **정보가 오직 색상만으로 전달되지 않게 하는 것**입니다. 만들고 있는 목업부터 시작해서 그 어떤 것이라도 이 기준이 적용되는 곳이라면 알아볼 수 있습니다. 입력 양식, 인포그래픽, 그래프, 태그, 상태 표시 등이 시작하기 좋은 곳입니다. 전자 상거래 웹사이트라면 제품의 색상 선택란도 알아보세요 (다음 장에서 더 알아봅시다). 그리고, 색맹 시뮬레이터를 통해 당신이 선택한 색이 여러 색맹 유형에 따라 어떻게 보여질 지 확인할 수 있습니다.

**[Color Oracle](https://colororacle.org/)**은 윈도, 맥, 리눅스에서 실행되는 무료 색맹 시뮬레이터입니다.

![](https://stephaniewalter.design/wp-content/uploads/2019/04/colorblindsimulator-oracle.jpg)

**[Stark](https://getstark.co/)**은 스케치(Sketch) 플러그인으로 여러 유형의 색맹을 가정해볼 수 있습니다.

*포토샵을 사용한다면, View > Proof Setup 에서 색맹 옵션을 선택해보세요.*

![](https://stephaniewalter.design/wp-content/uploads/2019/04/colorblindsimulator-stark-sketch.jpg)

**[Toptal’s colorfilter](https://www.toptal.com/designers/colorfilter)** 는 웹사이트를 테스트하는 온라인 도구로, 여러 유형의 색맹 사용자가 어떻게 페이지를 보게 될 것인지 보여줍니다.

![](https://stephaniewalter.design/wp-content/uploads/2019/04/colorblindsimulator-toptal.jpg)

## 명암비 확인을 위한 도구

두 번째 기준은 **문자열(전경 요소 포함)과 배경 사이의 명암비**입니다. 앞서 말했듯, 도움이 되는 여러 도구가 있어 직접 계산할 필요가 없습니다.

### 온라인 도구

**[Tanaguru Contrast Finder](http://contrast-finder.tanaguru.com/)**는 두 색상 사이의 명암비를 확인할 수 있을 뿐 아니라, 적합한 명암비를 확보하지 못한 경우에 새로운 색을 찾는 데 도움을 줍니다. 제가 쓴 [Tips to Create an Accessible and Contrasted Color Palette](https://stephaniewalter.design/blog/tips-create-accessible-color-palette/)를 통해서 더 알아보세요.

![](https://stephaniewalter.design/wp-content/uploads/2019/04/tanaguru.jpg)

**[Color Review](https://color.review/check/FEDC2A-5A3B5D)**를 통해 두 색상 사이의 명암비를 확인할 수 있습니다. 또한 색 조합이 어떻게 보일지 미리 확인할 수 있도록 보여줍니다. 적합하지 않은 색상을 골랐을 때는, 왼쪽의 색상 선택 도구를 통해 다른 대안을 찾을 수 있도록 도와줍니다.

![](https://stephaniewalter.design/wp-content/uploads/2019/04/color-review.jpg)

**[Contrast Ratio](https://contrast-ratio.com/)** 이 온라인 도구는 단순하지만 효율적인 방법으로 배경색에 대해 어떻게 문자열의 색상이 표시될지 보여줍니다.
 
![](https://stephaniewalter.design/wp-content/uploads/2019/04/contrast-ratio.jpg)

**[Colorable](http://jxnblk.com/colorable/demos/text/?background=%23123409&foreground=%23DACDCD)**도 문자열과 배경색 사이의 명암비를 확인하는 온라인 도구입니다. 문자열 색상과 배경색을 입력해 어떻게 보일지 확인할 수 있어 선호하는 도구입니다. 충분한 명암비가 나오지 않았을 때 색상, 채도, 밝기를 조절해 적합한 색을 찾을 수 있습니다.

![](https://stephaniewalter.design/wp-content/uploads/2019/04/colorable.jpg)

사이트 전체를 확인하고 싶으면 [Checkmycolours.com](http://www.checkmycolours.com/)에 URL을 입력해 사이트에 존재하는 모든 명암비 문제에 대한 결과를 얻을 수 있습니다. 가끔 정확한 배경을 얻어오지 못하는 경우가 있으니 사용에 주의해주세요.

### 설치해서 사용할 수 있는 오프라인 도구

**[Contrast Analyser](https://developer.paciellogroup.com/resources/contrastanalyser/)**는 윈도, 맥, 그리고 리눅스에 설치해서 사용하는 도구입니다. 색상 선택 도구에서 색을 골라 명암비를 확인할 수 있습니다. 주의를 기울여 색을 골라도 화면에 따라 정확한 16진수 값이 선택되지 않는 문제가 있어, 도구에 16진수 색상 값을 직접 “복사해서 붙여넣기”해서 쓰고 있습니다.

![](https://stephaniewalter.design/wp-content/uploads/2019/04/color-contrast-analyser.jpg)

맥 사용자라면 7 달러를 지불하고 [usecontrast.com](https://usecontrast.com/)를 쓸 수도 있지만, 저는 써보진 않았습니다.

## 제품 디자인의 색 접근성에 대한 글과 정보

도구에 대한 것은 알아봤으니, 이제 접근성을 가진 제품을 만들기 위한 몇 가지 글과 정보에 대해 알아봅시다.

### 접근성 높은 색 팔레트 만들기

**[90 combinations](http://clrs.cc/a11y/)**은 충분한 명암비를 가진 문자열과 배경색의 조합을 음, 허허, 90가지나 보여주는 페이지입니다. 일부는 18포인트 (굵은 문자열인 경우 14포인트) 이상에만 적용되는 4.1 AA의 큰 명암비를 가지고 있어 주의해서 사용해야 합니다. 아이디어가 떠오르지 않는다면 이 사이트에서 시작하는 것도 좋겠지만…

디자이너의 입장에서 보자면, 이 90가지 조합 중 절반은 사용하지 않는 것이 좋겠습니다. 노란색 바탕에 보라색 글씨나 보라색 바탕 위에 초록색 글씨는 4.5 이상의 명암비를 가지긴 하지만 읽기에 너무나도 불편한 조합입니다. 할 수 있다고 해서 꼭 해야 한다는 뜻은 아니니까요!

![](https://stephaniewalter.design/wp-content/uploads/2019/04/90accessible-color-combinations.jpg)

**[Accessible color palette builder](https://toolness.github.io/accessible-color-matrix/?n=white&n=Color%202&n=Color%203&n=Color%204&n=Color%205&v=FFFFFF&v=FEDC2A&v=5A3B5D&v=8B538F&v=C3A3C9) **는 제가 가장 선호하는 도구입니다. 최대 6가지 색상을 입력해서 만든 색상 행렬을 통해 어떤 색상을 조합할 수 있을지 알려줍니다.

![](https://stephaniewalter.design/wp-content/uploads/2019/04/color-matrix-accessibility.jpg)

6가지 색상보다 더 많은 색상으로 구성된 복잡한 행렬을 원한다면 [이 도구도 확인해보세요](http://jxnblk.com/colorable/demos/matrix/).

**[Contrast Grid](http://contrast-grid.eightshapes.com/?background-colors=%23FFFFFF%2C%20White%0D%0A%23FEDC2A%2C%20Yellow%0D%0A%235A3B5D%2C%20Dark%20Purple%0D%0A%238B538F%2C%20Light%20Purple%0D%0A%23C3A3C9%2C%20Lightst%20purple%0D%0A%23777777%2C%20Gray%0D%0A%23555555%2C%20Darker%20Gray%0D%0A%0D%0A&foreground-colors=%23FFFFFF%2C%20White%0D%0A%23FEDC2A%2C%20Yellow%0D%0A%235A3B5D%2C%20Dark%20Purple%0D%0A%238B538F%2C%20Light%20Purple%0D%0A%23C3A3C9%2C%20Lightst%20purple%0D%0A%23777777%2C%20Gray%0D%0A%23555555%2C%20Darker%20Gray%0D%0A%23444444%2C%20Darker%20%20Darker%20Gray%0D%0A%23333333%2C%20Fifty%20Shades%20of%20darker%20gray%0D%0A%23222222%2C%20Dorian%20Gray%3F&es-color-form__tile-size=regular)**는 전경색과 배경색의 조합을 격자로 표현하는 방식을 받아들여 한 단계 더 발전시켰습니다. 이 도구를 이용해서 행과 열에 원하는 색상을 선택하여 자신만의 격자를 만들 수 있습니다. ([Mickaël G.](https://twitter.com/StrapTrooper)가 알려주었습니다)

![](https://stephaniewalter.design/wp-content/uploads/2019/04/contrast-grid.jpg)

**[Cloudflare color tool](https://cloudflare.design/color/)** 음, 이건 정말 비직관적인 도구지만 강력하긴 합니다. 화면의 상단에서 URL을 입력하거나 이미지를 지정해 색상을 불러오거나, 색상 상자에서 직접 선택할 수도 있습니다. 색을 네 가지 분류(부모, 주 색상, 배경, 테두리)로 이리저리 움직여 확인해 보거나, “접근성 높은 조합(view accessible combinations” 링크를 사용해 접근성을 고려한 색의 조합을 확인할 수도 있습니다.

![](https://stephaniewalter.design/wp-content/uploads/2019/04/cloudfour-contrast-tool.jpg)

[My struggle with colors - Demystifying colors for accessible digital experiences](https://uxdesign.cc/my-struggle-with-colors-52156c664b87) 와 [My struggle with colors, part II - Building an accessible color system from scratch.](https://uxdesign.cc/my-struggle-with-colors-part-ii-ed71bff6302a)도 읽어보세요. 몇몇 프로젝트에서 5단계의 10가지 음영을 고르는 방법을 사용해봤는데, 꽤 괜찮았습니다.

### 색맹인 사람들이 콘텐츠를 더 잘 이해하도록 도움 주기

[We are Colorblind](https://wearecolorblind.com/)에 색맹을 이해하는 데 도움이 되는 여러 정보와 글, 그리고 예제가 있습니다.

![](https://stephaniewalter.design/wp-content/uploads/2019/04/wearecolorblind.jpg)

  * [Designing UI with Color Blind Users in Mind](https://www.secretstache.com/blog/designing-for-color-blind-users/) 패턴과 텍스쳐부터 기호와 라벨에 이르기까지 색맹 사용자를 위한 7가지 디자인 팁.
  * [Color Blindness Considerations for Designers and Content Managers](https://medium.com/@sheribyrnehaber/color-blindness-considerations-for-designers-and-content-managers-a767ab38a825?ref=heydesigner), 색맹을 대상으로 하는 디자인에 대한 몇 가지 간단한 팁.
  * [5 Ways to Improve Your Ecommerce Design for Colourblind Users](https://www.shopify.com/partners/blog/86314118-5-ways-to-improve-your-ecommerce-design-for-colourblind-users), 이것은 특히 전자 상거래에 유효한데, “화면상에서 서로 다른 색을 구분할 수 없다면 어떻게 티셔츠의 색상을 고를 수 있을까?” 등의 문제를 다루고 있습니다.
  * [Colorblind accessibility in video games – is the industry heading in the right direction?](http://www.gamersexperience.com/colorblind-accessibility-in-video-games-is-the-industry-heading-in-the-right-direction/)  게임 산업에서 일부 게임에서 색맹을 주요한 주제로 다루고 있는 것에 대한 흥미로운 글.

### Geri Coady가 제공해준 정보

Geri Coady는 뛰어난 디자이너로 도움이 될만한 여러 글을 잘 정리해두었습니다.

  * [Color Accessibility Workflows](https://abookapart.com/products/color-accessibility-workflows) Book Apart의 도서.
  * [A Pocket Guide To Colour Accessibility](http://hellogeri.com/blog/view/now_available_pocket_guide_to_colour_accessibility)라는 책을 쓰기도 했지만, 지금은 찾기 어렵습니다.
  * [Colour Accessibility](https://24ways.org/2012/colour-accessibility/), 기본이 되는 24가지 방법.

### 도움이 되는 몇 가지 글

마지막으로, 이 주제에 대해 좀 더 깊게 다루는 몇몇 글을 소개합니다.

  * [A guide to color accessibility in product design](https://www.invisionapp.com/inside-design/color-accessibility-product-design/) 시작하기에 도움이 되는 또 다른 글입니다.
  * [Color in Design Systems 16 Tips for Setting Up a System That Endures](https://medium.com/eightshapes-llc/color-in-design-systems-a1c80f65fa3)에서 제시하는 16가지 팁 중 13개가 접근성에 대한 이야기입니다.
  * [Color Contrast for Better Readability](https://www.viget.com/articles/color-contrast/) 접근성 높은 색 조합을 구축하는 데 도움이 되는 글입니다.
  * [Chrome DevTools: Accessible Colors](https://uxdesign.cc/chrome-devtools-accessible-colors-300ec462a63c)

공유할 만한 정보나 도구가 있다면 댓글로 알려주세요.

### 요청 받은 브랜딩을 진행하는 데 어려움이 있습니다. 도와주세요.

종종 클라이언트로부터 의뢰받은 브랜딩 작업을 할 때가 있을겁니다. 그들 중 몇몇은 웹사이트의 명암비 문제로 기업의 대표 색상을 바꾸자는 의견을 좋아하지 않을 수도 있습니다. 이런 경우에는 **[스타일 변환기를 사용해서 적합한 대안 버전을 제공하는 것](https://www.w3.org/TR/WCAG-TECHS/C29.html)**이 마지막 방법일 수 있습니다.

 *글을 검토하고 도구를 추천해준 [Geoffrey Crofte](https://twitter.com/geoffreycrofte)에게 감사드립니다.* 🙂

웹 사이트나 모바일 앱을 위한 UX나 UI 디자이너를 찾고 있나요? 컨퍼런스에서 발표하거나 그냥 저에 대해서 더 궁금하신가요? [제 포트폴리오](https://stephaniewalter.design/#work)를 둘러보고 저에게 연락해주세요.
