### 1. 명제 논리 (Propositional Logic)
* 부정 (Negation): $\neg P$
* 논리곱 (Conjunction): $P \land Q$
* 논리합 (Disjunction): $P \lor Q$
* 조건/함의 (Implication): $P \rightarrow Q$
* 쌍방조건 (Biconditional): $P \leftrightarrow Q$

### 2. 술어 논리 및 술어 논리식 (Predicate Logic)
* 술어 논리식 기본 형태: $P(x)$
* 전칭 양화사 (Universal Quantifier): $\forall x P(x)$
* 존재 양화사 (Existential Quantifier): $\exists x P(x)$

### 3. 논리식의 주요 동치 관계 (Logical Equivalences)
* 드모르간의 법칙 (De Morgan's Laws):
  * $\neg(P \land Q) \equiv \neg P \lor \neg Q$
  * $\neg(P \lor Q) \equiv \neg P \land \neg Q$
* 조건문 동치 (Implication Elimination):
  * $P \rightarrow Q \equiv \neg P \lor Q$
* 대우 법칙 (Contraposition):
  * $P \rightarrow Q \equiv \neg Q \rightarrow \neg P$
* 양화사 부정 법칙:
  * $\neg \forall x P(x) \equiv \exists x \neg P(x)$
  * $\neg \exists x P(x) \equiv \forall x \neg P(x)$

### 4. 논리곱 표준형 변환 (Conjunctive Normal Form, CNF)
1. 함의 기호 제거: $P \rightarrow Q \equiv \neg P \lor Q$
2. 부정 기호 이동 (드모르간 법칙 적용): $\neg(P \land Q) \equiv \neg P \lor \neg Q$
3. 분배법칙 적용 ($\lor$를 $\land$ 내부로 전개): $P \lor (Q \land R) \equiv (P \lor Q) \land (P \lor R)$
* 최종 형태 예시: $(A \lor \neg B) \land (B \lor C)$

### 5. 스콜렘 표준형 변환 (Skolem Normal Form)
* 앞에 전칭 양화사가 없는 존재 양화사 제거 (스콜렘 상수 대체):
  * $\exists x P(x) \Rightarrow P(c)$
* 앞에 전칭 양화사가 있는 존재 양화사 제거 (스콜렘 함수 대체):
  * $\forall x \exists y P(x, y) \Rightarrow \forall x P(x, f(x))$
  * $\forall x \forall y \exists z P(x, y, z) \Rightarrow \forall x \forall y P(x, y, g(x, y))$
