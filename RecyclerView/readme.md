## 리사이클러뷰
리사이클러뷰란 안드로이드 공식문서에선 "대규모 데이터셋을 제한된 범위에 제공하기 위한 유연한 뷰"라 정의되어있습니다.
리사이클러뷰는 기존에 리스트 형태의 화면 구성에 사용되는 리스트뷰에 *유연함 + 성능*을 더한 리스트뷰의 업그레이드 버전이라고 할 수 있습니다.

<img src="https://github.com/heetsamber/Andriod_Study/blob/main/RecyclerView/997123455C88BD1A01.png">
### 리사이클러뷰 구조
리사이클러뷰는 기본적으로 크게 4가지의 구조로 나뉘는데 

+ 리사이클러뷰(RecyclerView) android.support.v7.widget.RecyclerView
+ 어댑터(Adapter) android.support.v7.widget.RecyclerView.Adapter
+ 레이아웃 매니저(LayoutManager) android.support.v7.widget.RecyclerView.LayoutManager
+ 뷰홀더(ViewHolder) android.support.v7.widget.RecyclerView.ViewHolder

#### 리사이클러뷰
리사이클러뷰는 안드로이드에서 제공하는 위젯으로 사용자의 데이터를 리스트 형태로 화면에 표시하는 *컨테이너* 역할을 수행합니다.

#### 어댑터
리사이클러뷰에 표시될 아이템 뷰를 생성하는 역할은 어댑터가 담당합니다. 사용자 데이터를 받아 아이템 뷰를 만듭니다.

#### 레이아웃 매니저
레이아웃 매니저는 리사이클러뷰가 아이템을 화면에 표시할 때, 리사이클러뷰 내부에서 배치되는 형태를 관리하는 역할입니다.

#### 뷰홀더
뷰홀더는 화면에 표시되는 아이템 뷰를 저장하는 객체입니다. 어댑터에 의해 관리되고 어댑터에서 생상됩니다.(레이아웃 매니저의 아이템 뷰 재활용 정책에 따라)



### 리사이클러뷰 작성 순서
1. 리사이클러뷰 추가
2. 아이템 뷰 레이아웃 추가
3. 리사이클러뷰 어댑터 구현
4. 어댑터 레이아웃 매니저 지정
