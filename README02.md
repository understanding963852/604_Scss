# Partials(파샬-부분적인) 
# - 소스에 반복되는 부분들을 분산시켜서 모듈화 시키는 기능(관련된것끼리 묶어서 분리,분산하는것)
  - 파샬 파일명은 _로 시작하며(_파일명.scss)
  - 파샬 파일을 불러올때는 @import '파일명' (_,확장명없이) 경로는 상대경로를 사용한다.
# scss는 _로 시작하는 파일은 컴파일하지 않는다.


# 변수에 중복을 막을수 있는 방법  -- @use, @forward
# @use --> 많이 사용
# 구분하는 방법은 파일명을 이용한다. 
```
@use './partials/var';
@use './partials/var2';

h1{color:var2.$color-primary}
```

# as 를 이용하여 별명을 붙일수 있다.

```
@use './partials/var';
@use './partials/var2' as v2;

h1{color:v2.$color-primary}
```











