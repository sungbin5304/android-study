# android-study
android 공부할거야!

> [ios 공부할거야!](https://github.com/sungbin5304/ios-study)

-----

- [x] [Publishing to Maven Central](https://chris.banes.dev/publishing-to-maven-central/) 
- [x] 멀티 모듈 
- [x] ~~구현체~~
- [x] getSystemService context scope (use application or activity)
- [x] [di scope 범위 (activity, context)](https://hyperconnect.github.io/2020/07/28/android-dagger-hilt.html)
- [x] rx 구독 생명주기 관리
- [x] 패키지 구분은 비슷한 클래스끼리로 묶기
- [x] 엑티비티에서도 databinding 활용하기
- [x] 밑에 코드 이해하기 [[원본코드]](https://github.com/fornewid/android-animation-11p-more/blob/end/sample/src/main/java/soup/animation/sample/SplashActivity.kt#L17)
```kotlin
private val binding by viewBindings(SplashActivityBinding::inflate)

inline fun <reified VB : ViewBinding> Activity.viewBindings(
    crossinline inflater: (LayoutInflater) -> VB
): Lazy<VB> {
    return lazy(LazyThreadSafetyMode.NONE) {
        inflater.invoke(layoutInflater)
    }
}
```
- [x] [android:configChanges 속성](https://developer.android.com/guide/topics/resources/runtime-changes?hl=ko)
- [ ] [인텐드애서 newTask 관련 -> task 관련](https://developer.android.com/guide/components/activities/tasks-and-back-stack?hl=ko)
- [x] [Clean Architecture](https://codechacha.com/ko/android-clean-architecture/)
- [x] repository 폴더는 무슨 역할을 담는 폴더 일까?
- [x] \~\~Impl 클래스는 무슨 역할을 하는 클래스 일까?
- [ ] di(dagger2, hilt) 심화 학습 (50% 완료) -> 미디움 정리 필요
- [ ] windowSoftInputMode 관련 정보
- [ ] @Binds가 뭘 까? in Dagger2
- [ ] what is Observable in DataBidning
- [ ] ConstraintLayout 자세한 정보
- [x] ~~ReKotlin~~ (쓸 일이 있을까?)
- [x] ScopedStorage
- [x] [Delegates](https://medium.com/hongbeomi-dev/%EB%B2%88%EC%97%AD-%EB%82%B4%EC%9E%A5%EB%90%9C-delegates-2%ED%8E%B8-bc4a23cb6f10)
- [x] [레포지토리 패턴](https://devvkkid.tistory.com/196) / [The “Real” Repository Pattern in Android](https://proandroiddev.com/the-real-repository-pattern-in-android-efba8662b754)
- [x] [AAC ViewModel vs MVVM ViewModel](https://enant.tistory.com/49)
- [x] [MVVM 관련 정보](https://blog.yena.io/studynote/2019/03/16/Android-MVVM-AAC-1.html)
- [x] MVI 패턴
