DK����� ���̳ʸ���

download_blinky_LEDS.cmd
  -> LED�� �ֱ������� ������
download_uart_c_AutoCon.cmd
  -> BLE NUS�� Uart�� Bypass�����ش�.
      * ��) GPS Bypass
        �ܸ� : CMB �Է��Ͽ� GPS to NUS���� ��ȯ
        DK���� : uart_c_AutoCon\make_ble_app_uart_c_hex.cmd �� �����Ͽ� Auto Connect MAC Address�� ����
                   ��)set MAC_TO_CONNECT_NUS=F07FEB6BAE30
                   make_ble_app_uart_c_hex.cmd�� �����Ͽ� ���̳ʸ� ����.
                   download_uart_c_AutoCon.cmd�� �����Ͽ� DK���忡 �ٿ�ε�.
        ��� : DK���忡 ����� Virtual Uart Port�� GPS�� ������ �� �ִ�.
        build�ʿ�� : examples\ble_central\ble_app_uart_c������� ���� -> src_in_ble_app_uart_c.zip�� main.c�� sdk_config.h�� merge�Ѵ�.
                         MAC�� �����ϴ� ��ġ������ �����Ѵ�. (0xa1a2a3a4a5a6�� Target mac���� ����. Intel Hex �Ѷ��� Ȥ�� �ζ����� �����ؾ��Ѵ�.)
                           make_ble_app_uart_c_hex.cmd.old1 -> �Ѷ����� �����ϴ� base cmd
                           make_ble_app_uart_c_hex.cmd.old1 -> �ζ����� �����ϴ� base cmd