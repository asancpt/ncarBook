
---
#documentclass: book
#papersize: A4
#fontsize: 10pt
#documentclass: krantz
#geometry: "margin=4in"               
#geometry: "a4paper,left=1.5in,right=1.5in,top=1in,bottom=1in"
#geometry: "a4paper, nohead, nomarginpar, left=1.5in,right=1.5in,top=5in,bottom=3in,foot=1in"
#geometry: "a4paper, nohead, nomarginpar"
#geometry: "total={6.5in,8.75in}, top=1.2in, left=0.9in, includefoot"
#geometry: "a4paper, nohead, nomarginpar, left=1.5in,right=1.5in,top=1in,bottom=1in, includeheadfoot"
title: "R을 사용한 비구획분석"
author: "배균섭, 한성필, 윤석규, 조용순, 김형섭"
description: "이 책은 R 패키지를 사용하여 비구획분석을 쉽게 따라할 수 있도록 쓰여졌습니다.  값비싼 상용소프트웨어와 동일한 결과를 얻으면서, 한번 익혀두면 속도와 연속성 측면에서 잇점이 많은 것을 발견할 수 있을 것입니다.  무엇보다 무료로 사용할 수 있는 R기반의 공개 소프트웨어라는 점에서 많은 연구자 혹은 기관에서 손쉽게 설치하고 실행할 수 있으리라 생각됩니다."
date: "2019-11-06"
url: 'https\://asancpt.github.io/book-ncar/'
github-repo: asancpt/book-ncar
cover-image: assets/cover.jpg
bibliography: ["bib/manual.bib", "bib/packages.bib"]
documentclass: krantz
biblio-style: apalike
link-citations: yes
colorlinks: yes
fontsize: 12pt
header-includes:
  - \usepackage{kotex}
output:
  bookdown::pdf_book: 
    keep_tex: yes
    pandoc_args: --top-level-division=chapter
    toc_depth: 3
    toc_unnumbered: no
    toc_appendix: yes
    #template: null
    #dev: "cairo_pdf"
    #latex_engine: xelatex
    #includes:
    #  in_header: latex/preamble.tex
    #  before_body: latex/before_body.tex
    #  after_body: latex/after_body.tex
  bookdown::gitbook:
    df_print: kable
    css: css/style.css
    split_by: chapter
    config:
      toolbar:
        position: static
      toc:
        #collapse: chapter
        before: |
          <li><a href="./index.html">R을 사용한 비구획분석</a></li>
        after: |
          <li><a href="http://github.com/asancpt/book-ncar">book-ncar Github 저장소</a></li>
      #download: [pdf]
      edit:
        link: https://github.com/asancpt/book-ncar/edit/master/%s
        text: "Edit"
  bookdown::pdf_document2: default
  bookdown::tufte_book2: default
  html_document: 
    df_print: kable
  bookdown::html_chapters:
    css: css/style.css
  bookdown::epub_book:
    stylesheet: css/style.css
editor_options: 
  chunk_output_type: console
---





# Preface {-}

[<img src="assets/cover.jpg" style="max-width:20%;min-width:80px;float:right;margin: 10px 10px 5px 5px" alt="Github repo" />](https://github.com/asancpt/book-ncar)

이 책은 R을 사용하여 비구획분석을 수행할 수 있도록 소개할 것입니다. 
값비싼 상용 소프트웨어와 동일한 결과를 얻을 수 있음을 실제 임상시험 자료를 통해 반복적으로 확인하였습니다. 
숫자 계산 뿐만 아니라 시각화도 가능하여 농도-시간 곡선, 용량군 별 파라메터의 forest plot 등의 유용한 그림도 쉽게 그릴 수 있습니다.
CDISC SDTM 표준을 따르는 용어를 사용한 것도 큰 장점입니다.
비구획분석 후 생물학적동등성을 평가할 수 있는 패키지도 함께 개발되었습니다.

한번 익혀두면 속도와 연속성 측면에서 커다란 잇점이 있음을 것을 발견할 수 있을 것입니다. 
또한 재현가능한 연구를 보다 수월하게 구현할 수 있습니다.
무엇보다 무료로 사용할 수 있는 R기반의 공개 소프트웨어라는 점에서 학교, 연구소, 정부기관, 제약회사 등에서 라이센스 등의 제약 없이 손쉽게 설치하고 실행할 수 있으리라 생각됩니다.
책에 대한 피드백, 오탈자 신고 등은 [깃허브 저장소](https://github.com/asancpt/book-ncar/issues)에 남겨주십시오.

감사합니다.

2019-11-06  
서울아산병원 임상약리학과, 울산대학교 임상약리학교실  
교수 배균섭,  
한성필, 윤석규, 조용순, 김형섭

*배균섭*  
서울아산병원 임상약리학과 과장, 울산대학교 의과대학 임상약리학교실 교수입니다. 수십편의 논문을 저술하였고 20년 이상의 프로그래밍 경력을 갖고 있습니다.

*한성필*  
가톨릭의대 약리학교실 연구강사입니다. 부산대학교 의학전문대학원을 졸업하였습니다.

*윤석규*  
서울아산병원 임상약리학과 전공의입니다. 연세대학교 원주캠퍼스 의과대학을 졸업하였습니다.

*조용순*  
인제의대 약리학교실 조교수입니다. 중앙대학교 의학전문대학원을 졸업하였습니다.

*김형섭*  
서울아산병원 임상약리학과 전공의입니다. 고려대학교 의학전문대학원을 졸업하였습니다.

![Creative Commons License](assets/cc.png)  
이 저작물은 [크리에이티브 커먼즈 저작자표시-비영리-동일조건변경허락 4.0 국제 라이선스](http://creativecommons.org/licenses/by-nc-sa/4.0/) 에 따라 이용할 수 있습니다.

<!-- https://creativecommons.org/choose/?lang=ko -->

**감사의 글**

\BeginKnitrBlock{rmdnote}<div class="rmdnote">본 출판물은 2016-2019년도 정부(미래창조과학부)의 재원으로 한국연구재단 첨단 사이언스·교육 허브 개발 사업의 지원을 받아 수행된 연구입니다 (NRF-2016-936606).</div>\EndKnitrBlock{rmdnote}

\mainmatter
