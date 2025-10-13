## Team 37 OptimusPrime
|항목|내용|
|---|---|
|프로젝트명|VM별 AI 워크로드 에너지 사용량 예측모델 설계 및 개선 방안|
|프로젝트 키워드|AI workload, Power Attribution, Energy Prediction|
|트랙|연구|
|프로젝트멤버|[강시연](https://github.com/uoehisx), [김지윤](https://github.com/horokkk), [신우림](https://github.com/RainyForest23)|
|팀지도교수|반효경 교수님|
|무엇을 만들고자 하는가|Energy Attribution Algorithm, Energy Profiling Engine, Lightweight Monitoring System, Validation Framework|
|고객|클라우드/서버에 별도의 비용을 지불하고 사용중인 기업들 |
|Pain Point|- 생성형 AI의 확산으로 데이터 센터 에너지 사용 급증<br> - GPU 연산 집중, 대규모 파라미터 이동, 고빈도 I/O로 기존 워크로드와는 상이한 자원별(CPU, GPU, 메모리, 스토리지) 에너지 사용 패턴 및 에너지 병목 발생<br> - 불공정한 과금체계|
|사용할 소프트웨어 패키지의 명칭과 핵심기능/용도, 사용시나리오|- Ubuntu 22.04 LTS : 시스템 기본 운영체제 <br> - qemu-kvm :가상머신 에뮬레이션 및 하드웨어 가상화 수행 <br> - libvirt-daemon-system & libvirt-python : VM 관리 및 Python 환경에서 libvirt API 호출 <br> - RAPL : CPU 전력 및 에너지 계측 <br> - nvidia-ml-py3 : GPU 전력 및 상태 모니터링 <br> - msr-tool : Model-Specification Register 접근 도구 <br> - virsh : VM 명령 제어 & 상태조회 <br> - perf : 커널 이벤트/CPU 성능 계측 <br> - psutil :  프로세스 및 시스템 리소스 모니터링 <br> - pandas : 시계열/테이블 데이터 처리 <br> - numpy : 배열 기반 수치 연산 <br> - scikit-learn : 머신러닝 알고리즘 라이브러리 <br> - grafana : 시계열 데이터 시각화 및 대시보드 <br> - seaborn : 통계적 시각화 <br> - matplotlib :2D 플롯 시각화 <br> - influx DB : 시계열 데이터 저장,쿼리 <br> - Pytorch : 딥러닝 모델 학습&추론 <br> - Tensorflow : 딥러닝 프레임워크|
|사용할 소프트웨어 패키지의 명칭과 URL|- Ubuntu 22.04 LTS : [https://releases.ubuntu.com/jammy/](https://releases.ubuntu.com/jammy/) <br> - qemu-kvm : [https://www.qemu.org/download/](https://www.qemu.org/download/) <br> - libvirt-daemon-system & libvirt-python : [https://libvirt.org/](https://libvirt.org/) <br> - RAPL : [https://www.kernel.org/doc/html/latest/power/rapl.html](https://www.kernel.org/doc/html/latest/power/rapl.html) <br> - nvidia-ml-py3 : [https://pypi.org/project/nvidia-ml-py3/](https://pypi.org/project/nvidia-ml-py3/) <br> - msr-tools : [https://github.com/intel/msr-tools](https://github.com/intel/msr-tools) <br> - virsh : [https://libvirt.org/manpages/virsh.html](https://libvirt.org/manpages/virsh.html) <br> - perf : [https://perf.wiki.kernel.org/index.php/Main_Page](https://perf.wiki.kernel.org/index.php/Main_Page) <br> - psutil : [https://pypi.org/project/psutil/](https://pypi.org/project/psutil/) <br> - pandas : [https://pandas.pydata.org/](https://pandas.pydata.org/) <br> - numpy : [https://numpy.org/](https://numpy.org/) <br> - scikit-learn : [https://scikit-learn.org/](https://scikit-learn.org/) <br> - grafana : [https://grafana.com/](https://grafana.com/) <br> - seaborn : [https://seaborn.pydata.org/](https://seaborn.pydata.org/) <br> - matplotlib : [https://matplotlib.org/](https://matplotlib.org/) <br> - influx DB : [https://www.influxdata.com/](https://www.influxdata.com/) <br> - Pytorch : [https://pytorch.org/](https://pytorch.org/) <br> - Tensorflow : [https://www.tensorflow.org/](https://www.tensorflow.org/) <br>
|
|팀그라운드룰|[GroundRule_OptimusPrime](https://github.com/Team37-OptimusPrime/optimusprime/blob/main/GroundRule.md)|
|최종수정일|2025-10-13|
