***
## SOPT FIRST WEEK


**ConstraintLayout 심화학습**

 - ConstraintDimentionRatio 이용해서 이미지를 1:1 비율로 만들어 줌 
 
 **GuideLine 이란 ?**
 
 - 화면 끝까지 글이 가지 않고 개행이 되는 기능
 - xml.code 

	    <androidx.constraintlayout.widget.Guideline  
			  android:id="@+id/guideline"  
			  android:layout_width="0dp"  
			  android:layout_height="0dp"  
			  android:orientation="vertical"  
			  app:layout_constraintGuide_percent="0.8">  
  
		</androidx.constraintlayout.widget.Guideline>

 - Guideline 만들어준 뒤에 적용하고 싶은 TextView에 넣어주기
 - Guideline 적용해준 TextView code
 - Layout_width와 Layout_height 속성은 match_parent, wrap_content, match_constraint로 해주기 
 - marginTop은 근처에 있는 뷰와 해주기 (수정하기 편함)  
 

	    app:layout_constraintEnd_toStartOf="@+id/guideline"  
		app:layout_constraintHorizontal_bias="0.0"  
		app:layout_constraintRight_toRightOf="@id/guideline"  
		app:layout_constraintStart_toStartOf="@+id/textView"  
		app:layout_constraintTop_toBottomOf="@+id/textView"

![Screenshot_1590599682](https://user-images.githubusercontent.com/58849278/83053758-313a6e80-a08c-11ea-88b1-7380552f6808.png)

