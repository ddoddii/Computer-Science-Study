## Python

- **파이썬에서 multiprocess 를 생성하는 방법은?**
  - `spawn` : python 인터프리터를 처음부터 생성하고, 라이브러리도 처음부터 import 해서 생성 속도가 느리다.
  - `fork` : os 에서 제공하는 `os.fork()` 를 사용한다. spawn 보다는 오버헤드가 적지만, thread 를 사용하는 상황에서 안전하게 메모리를 복사할 수 없어서 문제를 일으킬 수 있습니다.
- **파이썬 object 란 어떤 정보를 담고 있나요?**
  - ID: unique identifier of the object
  - value: what data the object actually stores (e.g. an integer, string, ...)
  - type: the data type of the value (int, boolean, string, ...)
  - reference count: how many times the object is references/used
- **GIL에 대해 설명해주세요. 🚨**
  - Python 의 Global Interpreter Lock 으로, 여러개의 스레드가 파이썬 코드를 한번에 하나만 사용할 수 있게 락을 거는 것이다.
  - Cpython 인터프리터가 threading lock 을 구현한 것이다 → 오직 하나의 쓰레드만 락을 획득할 수 있다.
  -
- **GIL이 없는 파이썬은 어떻게 동작하나요?**
  - no-GIL 파이썬은 여러 기법을 함께 사용해서 참조 카운팅의 스레드 안정성을 확보하면서, 싱글 스레드 프로그램의 속도에는 영향을 주지 않거나 영향을 최소화합니다.
- **List와 Tuple의 차이에 대해 설명해주세요.**
- **파이썬 코루틴에 대해 아는대로 설명해주세요.**
- **파이썬 데코레이터에 대해 아는대로 설명해주세요.**
- **MRO에 대해 설명해주세요.**
- **Magic Method에 대해 설명해주세요.**
- **new**와 **init**의 차이에 대해 설명해주세요.
- **repr**와 **str**의 차이에 대해 설명해주세요.
- **r string과 u string에 대해 설명해주세요.**
- **Call by Assignment에 대해 설명해주세요.**
- **파이썬에서의 접근제어 지시자에 대해 아는대로 설명해주세요.**
- **global과 nonlocal 키워드의 차이에 대해 설명해주세요.**
- **classmethod와 staticmethod의 차이에 대해 설명해주세요.
  기**
- **파이썬의 GC 에 대해 설명해주세요.**
