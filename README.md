# Code Peer Review Templete

- 코더 : 조웅제, 전진환
- 리뷰어 : 이영빈


# PRT(PeerReviewTemplate)

각 항목을 스스로 확인하고 체크하고 확인하여 작성한 코드에 적용하세요.

- [ ] 1.코드가 정상적으로 동작하나요?

  > 정상적으로 작동하지 않았으며 제대로 구현되지 못했습니다.

- [x] 2.문제를 제대로 이해했나요?

  > 컨셉에 대해서 이해는 완료했습니다.
  >
  > 1. map을 구현 (1 ~ 100)
  >
  > 2. 주사위를 구현 (random하게 1 - 6)
  >
  > 3. 사다리와 뱀은 goto로 구현할 예정
  >
  >    ```python
  >    class Game:
  >      def __init__(self, name):
  >        self.name = name  
  >        self.player = {}
  >        self.player[name] = 0
  >        
  >      def dIce(self):
  >        self.number = random.randint(1, 6)
  >        return self.number
  >      
  >      def goto(self):
  >        #함정, 사다리 만났을 때 이동하는 경우의 수 
  >        pass  
  >        
  >      def move(self):
  >        self.player[self.name] += self.dice()
  >    
  >      def end(self):
  >        if self.player[self.name] < 100:
  >          print("end")
  >    ```
  >
  >    

- [ ] 3.함수가 작동하는 방식을 잘 설명했나요?

  > 함수가 작동하는 방식에 대해 제대로 설명하지 못했습니다.
  >
  > 특히 dice에서의 오타를 발견하지 못했습니다. 

- [ ] 4.발생 가능한 에러를 찾아서 디버깅을 했나요?

  > '오타'라는 발생 가능한 에러를 시간 안에 찾지 못했고 디버깅하지 못했습니다.
  >
  > ```python
  > def dIce(self):
  >     self.number = random.randint(1, 6)
  >     return self.number
  >     
  > A.dice
  > ```
  >
  > 

- [ ] 5.코드를 더 개선시켰나요?

  > 원 코드가 존재하지 않고 리팩토링이 들어가는 상황이 아니기 때문에 해당 사항은 판단할 수 없습니다. 그럼에도 전체적인 코드를 class함수로 만들어서 작성하려고 했다는 점에서 부분점수를 드리고 싶습니다.
  >
  > ```python
  > class Game:
  >   def __init__(self, name):
  >     self.name = name  
  >     self.player = {}
  >     self.player[name] = 0
  >     
  >   def dIce(self):
  >     self.number = random.randint(1, 6)
  >     return self.number
  >   
  >   def goto(self):
  >     #함정, 사다리 만났을 때 이동하는 경우의 수 
  >     pass  
  >     
  >   def move(self):
  >     self.player[self.name] += self.dice()
  > 
  >   def end(self):
  >     if self.player[self.name] < 100:
  >       print("end")
  > ```
  >
  > 

