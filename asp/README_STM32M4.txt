
	TOPPERS/ASP Kernel��Release 1.9.7��STM32F4/L4/WB/DK2
		Toyohashi Open Platform for Embedded Real-Time Systems/
		Advanced Standard Profile Kernel

TOPPERS/ASP STM32M4�ϰʲ���10�Υܡ��ɤ�GCC�γ�ȯ�Ķ����б����ޤ���
�ܥѥå������ϸ��̥ѥå������Ǥ��뤿�ᡢTOPPERS/ASP�����ͥ륿�����å�
���¸���ѥå�����asp-1.9.3.tar.gz���Ȥ߹�碌�ƻ��Ѥ��Ƥ���������
(1)STM�� STM32F4 Discovery�ܡ���
   Chip:STM32F407VGT6
(2)Olimex��STM32-E407�ܡ���
   Chip:STM32F407ZGT6
(3)�����ƥ��Υ��Ҥ�stm32f429�ܡ���
   Chip:STM32F429
(4)STM��STM32F401 Nucleo�ܡ���
   Chip:STM32F401RET6
(5)STM��STM32F446 Nucleo-64�ܡ���
   Chip:STM32F446RET6
(6)STM��STM32F446 Nucleo-144�ܡ���
   Chip:STM32F446ZET6
(7)STM��STM32L476 Nucleo-64�ܡ���
   Chip:STM32L476RGT6
(8)STM��STM32L476 Discovery�ܡ���
   Chip:STM32L476VGT6
(9)STM��STM32L4R5 Nucleo-144�ܡ���
   Chip:STM32L4R5ZIT6
(10)STM��STM32WB55 Nucleo�ܡ���
   Chip:STM32WB55RGV6
(11)STM��STM32G474 Nucleo-64�ܡ���
   Chip:STM32G474RET6
(12)STM��STM32G431 Nucleo-64�ܡ���
   Chip:STM32G431RBT6
(13)STM��STM32MP157C-DK2�ܡ��� cortexm4
   Chip:STM32M4

ASP�μ¹Է��֤ϰʲ��Σ��Ĥ򥵥ݡ��Ȥ��ޤ���
�¹Է��֤ϡ�����ѥ�������ѿ�DBGENV��������ѹ����Ǥ��ޤ���
Makefile��������ѹ����Ǥ��ޤ���

(1)RAM�¹ԡ�ROM��˥�(rommon)�ǵ�ư�����ܡ��ɤˡ�UART���Ѥ���
ASP�μ¹Է���(srec)���������ɤ��Ƽ¹Ԥ������
rommon��FLASH ROM����ߥե������tools/rommon���֤��Ƥ���ޤ���
DBGENV�����ꤵ��ʤ���硢�ޤ���RAM������ξ�硢���η��֤Υӥ�ɤ�Ԥ��ޤ���

(2)ROM�¹ԡ�FLASH ROM�˽񤭹���Ǽ¹Ԥ������
DBGENV��ROM������ξ�硢���η��֤Υӥ�ɤ�Ԥ��ޤ���

STM��STM32F401 Nucleo�ܡ��ɤ˴ؤ��Ƥϡ�TrueSTUDIO�Υץ������ȥե������
tools/TrueSTUDIO���Ѱդ��Ƥ��ޤ���
����ˤ�ꡢľ��TrueSTUDIO���Ѥ��ƥӥ�ɤ���ǽ�Ǥ���
�¹Է��֤�ROM�¹Ԥ˸���Ǥ���

�ڥǥ��쥯�ȥ깽����

arch/arm_m_gcc/common
	cortex-m�Υ������
arch/arm_m_gcc/stm32f4xx
	stm32f4��chip��¸��
arch/arm_m_gcc/stm32l4xx
	stm32l4��chip��¸��
arch/gcc
	gcc�δĶ���
target/stm32e407_gcc
	STM32-E407�ܡ��ɤΥ������åȰ�¸��
target/stm32f4discovery_gcc
	STM32F4 Discovery�ܡ��ɤΥ������åȰ�¸��
target/stm32f401nucleo_gcc
	STM32F401 Nucleo�ܡ��ɤΥ������åȰ�¸��
target/stm32f429board_gcc
	stm32f429�ܡ��ɤΥ������åȰ�¸��
target/stm32f446nucleo64_gcc
	stm32f446 Nucleo-64�ܡ��ɤΥ������åȰ�¸��
target/stm32f446nucleo144_gcc
	stm32f446 Nucleo-144�ܡ��ɤΥ������åȰ�¸��
target/stm32l476nucleo64_gcc
	stm32l476 Nucleo-64�ܡ��ɤΥ������åȰ�¸��
target/stm32l476discovery_gcc
	stm32l476 discovery�ܡ��ɤΥ������åȰ�¸��
target/stm32l4r5nucleo144_gcc
	stm32l4r5 Nucleo-144�ܡ��ɤΥ������åȰ�¸��
target/stm32wb55nucleo_gcc
	stm32wb55 Nucleo�ܡ��ɤΥ������åȰ�¸��
target/stm32g474nucleo64_gcc
	stm32g474 Nucleo-64�ܡ��ɤΥ������åȰ�¸��
target/stm32g431nucleo64_gcc
	stm32g431 Nucleo-64�ܡ��ɤΥ������åȰ�¸��
target/stm32mp157cdk2_gcc
	stm32mp157cdk2�ܡ��ɤ�cortexM4�����������åȰ�¸��
tools/rommon
	ROM��˥���UART���������ROM��˥��񤭹��ߥХ��ʥ�ե�����
	ROM��˥��Υ�������TOPPERS���饳��ƥ�Ĵ��ã�������
	STM32F401-Nucleo 64�ܡ����Ԥˤ����ۤ��ޤ���
tools/TrueSTUDIO
	STM32F401 Nucleo�ܡ����Ѥ�TrueSTUDIO�Υץ������ȥե�����

1.9.x �С����������
	2016ǯ01��03��	Release	1.9.2		�ǽ�Υ�꡼��
	2016ǯ07��22��	Release	1.9.3		STM32F446 nucleo 64/144�ܡ����б�
	2017ǯ08��28��	Release	1.9.4		STM32L476 �ܡ����б�
	2019ǯ02��04��	Release	1.9.5		STM32L4R5 nucleo 144 �ܡ����б�
	2019ǯ12��19��	Release	1.9.6		STM32WB55 nucleo �ܡ����б�
	                             		STM32G474/STM32G431 nucleo 64  �ܡ����б�
	2021ǯ03��08��	Release	1.9.7		STM32MP157C-DK2 �ܡ��� cortexM4�����б�
										STM32WB55 nucleo �ܡ���BLE�б������ӥ��������ɲ�

