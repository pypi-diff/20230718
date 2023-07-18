# Comparing `tmp/SpiNNMan-2016.001.zip` & `tmp/SpiNNMan-3.0.0.zip`

## zipinfo {}

```diff
@@ -1,247 +1,249 @@
-Zip file size: 232537 bytes, number of entries: 245
--rw-rw-rw-  2.0 fat      268 b- defN 16-Apr-28 13:51 SpiNNMan-2016.001/PKG-INFO
--rw-rw-rw-  2.0 fat     1344 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/README
--rw-rw-rw-  2.0 fat       64 b- defN 16-Apr-28 13:51 SpiNNMan-2016.001/setup.cfg
--rw-rw-rw-  2.0 fat     1658 b- defN 16-Apr-19 14:01 SpiNNMan-2016.001/setup.py
--rw-rw-rw-  2.0 fat     5368 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/constants.py
--rw-rw-rw-  2.0 fat     7813 b- defN 16-Apr-22 09:44 SpiNNMan-2016.001/spinnman/exceptions.py
--rw-rw-rw-  2.0 fat   132264 b- defN 16-Apr-22 09:44 SpiNNMan-2016.001/spinnman/transceiver.py
--rw-rw-rw-  2.0 fat     5441 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/__init__.py
--rw-rw-rw-  2.0 fat     1836 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/connections/connection_listener.py
--rw-rw-rw-  2.0 fat    10125 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/connections/scp_request_pipeline.py
--rw-rw-rw-  2.0 fat     1123 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/connections/socket_address_with_chip.py
--rw-rw-rw-  2.0 fat     1644 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/connections/token_bucket.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/connections/__init__.py
--rw-rw-rw-  2.0 fat      816 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_connection.py
--rw-rw-rw-  2.0 fat     1450 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_eieio_receiver.py
--rw-rw-rw-  2.0 fat      761 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_eieio_sender.py
--rw-rw-rw-  2.0 fat      656 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_listenable.py
--rw-rw-rw-  2.0 fat     1903 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_multicast_receiver.py
--rw-rw-rw-  2.0 fat     1275 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_multicast_sender.py
--rw-rw-rw-  2.0 fat     1681 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_scp_receiver.py
--rw-rw-rw-  2.0 fat     1826 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_scp_sender.py
--rw-rw-rw-  2.0 fat     1385 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_sdp_receiver.py
--rw-rw-rw-  2.0 fat      729 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_sdp_sender.py
--rw-rw-rw-  2.0 fat     1482 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_spinnaker_boot_receiver.py
--rw-rw-rw-  2.0 fat      839 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_spinnaker_boot_sender.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/connections/abstract_classes/__init__.py
--rw-rw-rw-  2.0 fat     3348 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_bmp_connection.py
--rw-rw-rw-  2.0 fat     2749 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_boot_connection.py
--rw-rw-rw-  2.0 fat     9565 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_connection.py
--rw-rw-rw-  2.0 fat     2452 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_eieio_connection.py
--rw-rw-rw-  2.0 fat     1073 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_ip_address_connection.py
--rw-rw-rw-  2.0 fat     2702 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_scamp_connection.py
--rw-rw-rw-  2.0 fat     3045 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_sdp_connection.py
--rw-rw-rw-  2.0 fat      615 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_utils.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/__init__.py
--rw-rw-rw-  2.0 fat      800 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/multicast_message.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/__init__.py
--rw-rw-rw-  2.0 fat     3902 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/create_eieio_command.py
--rw-rw-rw-  2.0 fat    16418 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/create_eieio_data.py
--rw-rw-rw-  2.0 fat      458 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/eieio/eieio_prefix.py
--rw-rw-rw-  2.0 fat     1316 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/eieio/eieio_type.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/eieio/__init__.py
--rw-rw-rw-  2.0 fat      170 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/eieio/abstract_messages/abstract_eieio_message.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/eieio/abstract_messages/__init__.py
--rw-rw-rw-  2.0 fat     1207 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/database_confirmation.py
--rw-rw-rw-  2.0 fat     1593 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/eieio_command_header.py
--rw-rw-rw-  2.0 fat     1537 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/eieio_command_message.py
--rw-rw-rw-  2.0 fat      581 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/event_stop_request.py
--rw-rw-rw-  2.0 fat     5604 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/host_data_read.py
--rw-rw-rw-  2.0 fat     1781 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/host_send_sequenced_data.py
--rw-rw-rw-  2.0 fat      583 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/padding_request.py
--rw-rw-rw-  2.0 fat     1977 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/spinnaker_request_buffers.py
--rw-rw-rw-  2.0 fat     8225 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/spinnaker_request_read_data.py
--rw-rw-rw-  2.0 fat      662 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/start_requests.py
--rw-rw-rw-  2.0 fat      636 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/stop_requests.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/__init__.py
--rw-rw-rw-  2.0 fat      720 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/abstract_eieio_data_element.py
--rw-rw-rw-  2.0 fat     8094 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_data_header.py
--rw-rw-rw-  2.0 fat     6851 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_data_message.py
--rw-rw-rw-  2.0 fat     1210 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_key_data_element.py
--rw-rw-rw-  2.0 fat     1648 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_key_payload_data_element.py
--rw-rw-rw-  2.0 fat     1338 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_without_payload_data_message.py
--rw-rw-rw-  2.0 fat     1844 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_with_payload_data_message.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/__init__.py
--rw-rw-rw-  2.0 fat      802 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_data_message.py
--rw-rw-rw-  2.0 fat      977 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_lower_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat      949 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_payload_prefix_data_message.py
--rw-rw-rw-  2.0 fat     1136 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_payload_prefix_lower_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat     1306 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_payload_prefix_upper_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat      979 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_timed_payload_prefix_data_message.py
--rw-rw-rw-  2.0 fat     1139 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_timed_payload_prefix_lower_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat     1275 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_timed_payload_prefix_upper_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat     1162 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_upper_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/__init__.py
--rw-rw-rw-  2.0 fat      865 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_data_message.py
--rw-rw-rw-  2.0 fat     1015 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_lower_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat     1033 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_payload_prefix_data_message.py
--rw-rw-rw-  2.0 fat     1162 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_payload_prefix_lower_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat     1299 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_payload_prefix_upper_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat      959 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_timed_data_message.py
--rw-rw-rw-  2.0 fat     1136 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_timed_lower_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat     1272 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_timed_upper_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat     1186 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_upper_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/__init__.py
--rw-rw-rw-  2.0 fat      801 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_data_message.py
--rw-rw-rw-  2.0 fat      977 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_lower_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat      949 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_payload_prefix_data_message.py
--rw-rw-rw-  2.0 fat     1137 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_payload_prefix_lower_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat     1305 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_payload_prefix_upper_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat     1012 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_timed_payload_prefix_data_message.py
--rw-rw-rw-  2.0 fat     1172 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_timed_payload_prefix_lower_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat     1274 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_timed_payload_prefix_upper_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat     1113 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_upper_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/__init__.py
--rw-rw-rw-  2.0 fat      830 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_data_message.py
--rw-rw-rw-  2.0 fat     1015 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_lower_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat     1033 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_payload_prefix_data_message.py
--rw-rw-rw-  2.0 fat     1162 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_payload_prefix_lower_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat     1298 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_payload_prefix_upper_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat      946 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_timed_data_message.py
--rw-rw-rw-  2.0 fat     1135 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_timed_lower_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat     1271 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_timed_upper_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat     1185 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_upper_key_prefix_data_message.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/__init__.py
--rw-rw-rw-  2.0 fat      664 b- defN 16-Jan-18 10:20 SpiNNMan-2016.001/spinnman/messages/scp/scp_alloc_free_type.py
--rw-rw-rw-  2.0 fat      465 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/scp/scp_bmp_info_type.py
--rw-rw-rw-  2.0 fat     1265 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/scp/scp_command.py
--rw-rw-rw-  2.0 fat      683 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/scp/scp_dpri_command.py
--rw-rw-rw-  2.0 fat      427 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/scp/scp_dpri_packet_type_flags.py
--rw-rw-rw-  2.0 fat      363 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/scp/scp_iptag_command.py
--rw-rw-rw-  2.0 fat      410 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/scp/scp_led_action.py
--rw-rw-rw-  2.0 fat      396 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/scp/scp_power_command.py
--rw-rw-rw-  2.0 fat     2013 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/scp/scp_request_header.py
--rw-rw-rw-  2.0 fat     1095 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/scp/scp_response_header.py
--rw-rw-rw-  2.0 fat     1002 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/scp/scp_result.py
--rw-rw-rw-  2.0 fat     1411 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/scp/scp_signal.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/__init__.py
--rw-rw-rw-  2.0 fat      355 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/abstract_messages/abstract_scp_bmp_reponse.py
--rw-rw-rw-  2.0 fat     1771 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/abstract_messages/abstract_scp_bmp_request.py
--rw-rw-rw-  2.0 fat     3696 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/abstract_messages/abstract_scp_request.py
--rw-rw-rw-  2.0 fat     2218 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/abstract_messages/abstract_scp_response.py
--rw-rw-rw-  2.0 fat       24 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/abstract_messages/__init__.py
--rw-rw-rw-  2.0 fat     1795 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_application_run_request.py
--rw-rw-rw-  2.0 fat     1511 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_app_stop_request.py
--rw-rw-rw-  2.0 fat     1793 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_bmp_set_led_request.py
--rw-rw-rw-  2.0 fat     1142 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_bmp_version_request.py
--rw-rw-rw-  2.0 fat     1103 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_check_ok_response.py
--rw-rw-rw-  2.0 fat     1595 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_count_state_request.py
--rw-rw-rw-  2.0 fat     1130 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_count_state_response.py
--rw-rw-rw-  2.0 fat     1454 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_dpri_exit_request.py
--rw-rw-rw-  2.0 fat     1415 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_dpri_get_status_request.py
--rw-rw-rw-  2.0 fat     1169 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_dpri_get_status_response.py
--rw-rw-rw-  2.0 fat     1520 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_dpri_reset_counters_request.py
--rw-rw-rw-  2.0 fat     1948 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_dpri_set_reinjection_packet_types.py
--rw-rw-rw-  2.0 fat     1919 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_dpri_set_router_emergency_timeout_request.py
--rw-rw-rw-  2.0 fat     1835 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_dpri_set_router_timeout_request.py
--rw-rw-rw-  2.0 fat     2225 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_flood_fill_data_request.py
--rw-rw-rw-  2.0 fat     1951 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_flood_fill_end_request.py
--rw-rw-rw-  2.0 fat     2091 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_flood_fill_start_request.py
--rw-rw-rw-  2.0 fat     1270 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_iptag_clear_request.py
--rw-rw-rw-  2.0 fat     1350 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_iptag_get_request.py
--rw-rw-rw-  2.0 fat     4192 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_iptag_get_response.py
--rw-rw-rw-  2.0 fat     1226 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_iptag_info_request.py
--rw-rw-rw-  2.0 fat     1563 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_iptag_info_response.py
--rw-rw-rw-  2.0 fat     1778 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_iptag_set_request.py
--rw-rw-rw-  2.0 fat     1521 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_iptag_tto_request.py
--rw-rw-rw-  2.0 fat     1705 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_led_request.py
--rw-rw-rw-  2.0 fat     1477 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_power_request.py
--rw-rw-rw-  2.0 fat      959 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_adc_request.py
--rw-rw-rw-  2.0 fat     1060 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_adc_response.py
--rw-rw-rw-  2.0 fat     1421 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_fpga_register_request.py
--rw-rw-rw-  2.0 fat     1189 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_fpga_register_response.py
--rw-rw-rw-  2.0 fat     1838 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_link_request.py
--rw-rw-rw-  2.0 fat     1465 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_link_response.py
--rw-rw-rw-  2.0 fat     1969 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_memory_request.py
--rw-rw-rw-  2.0 fat     1312 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_memory_response.py
--rw-rw-rw-  2.0 fat     2179 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_reverse_iptag_set_request.py
--rw-rw-rw-  2.0 fat     1657 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_router_alloc_request.py
--rw-rw-rw-  2.0 fat     1134 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_router_alloc_response.py
--rw-rw-rw-  2.0 fat     1405 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_router_clear_request.py
--rw-rw-rw-  2.0 fat     2791 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_router_init_request.py
--rw-rw-rw-  2.0 fat     2266 b- defN 16-Apr-19 14:13 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_sdram_alloc_request.py
--rw-rw-rw-  2.0 fat     1598 b- defN 16-Apr-19 14:14 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_sdram_alloc_response.py
--rw-rw-rw-  2.0 fat     2397 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_sdram_de_alloc_request.py
--rw-rw-rw-  2.0 fat     1561 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_sdram_de_alloc_response.py
--rw-rw-rw-  2.0 fat     1819 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_send_signal_request.py
--rw-rw-rw-  2.0 fat     1603 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_version_request.py
--rw-rw-rw-  2.0 fat     1185 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_version_response.py
--rw-rw-rw-  2.0 fat     1749 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_write_fpga_register_request.py
--rw-rw-rw-  2.0 fat     2063 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_write_link_request.py
--rw-rw-rw-  2.0 fat     2037 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_write_memory_request.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-2016.001/spinnman/messages/scp/impl/__init__.py
--rw-rw-rw-  2.0 fat      448 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/sdp/sdp_flag.py
--rw-rw-rw-  2.0 fat     9257 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/messages/sdp/sdp_header.py
--rw-rw-rw-  2.0 fat     1735 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/sdp/sdp_message.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/sdp/__init__.py
--rw-rw-rw-  2.0 fat     3242 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/spinnaker_boot/spinnaker_boot_message.py
--rw-rw-rw-  2.0 fat     6355 b- defN 16-Mar-16 11:24 SpiNNMan-2016.001/spinnman/messages/spinnaker_boot/spinnaker_boot_messages.py
--rw-rw-rw-  2.0 fat      430 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/spinnaker_boot/spinnaker_boot_op_code.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/spinnaker_boot/__init__.py
--rw-rw-rw-  2.0 fat    24328 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/spinnaker_boot/boot_data/scamp-133.boot
--rw-rw-rw-  2.0 fat    14286 b- defN 16-Apr-01 15:01 SpiNNMan-2016.001/spinnman/messages/spinnaker_boot/_system_variables/_system_variable_boot_values.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/messages/spinnaker_boot/_system_variables/__init__.py
--rw-rw-rw-  2.0 fat     3767 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/model/adc_info.py
--rw-rw-rw-  2.0 fat     1306 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/model/bmp_connection_data.py
--rw-rw-rw-  2.0 fat     8633 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/model/chip_info.py
--rw-rw-rw-  2.0 fat     2822 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/model/core_subset.py
--rw-rw-rw-  2.0 fat     4620 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/model/core_subsets.py
--rw-rw-rw-  2.0 fat     7667 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/model/cpu_info.py
--rw-rw-rw-  2.0 fat      587 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/model/cpu_state.py
--rw-rw-rw-  2.0 fat     9054 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/model/diagnostic_filter.py
--rw-rw-rw-  2.0 fat      555 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/model/diagnostic_filter_default_routing_status.py
--rw-rw-rw-  2.0 fat      859 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/model/diagnostic_filter_destination.py
--rw-rw-rw-  2.0 fat     1011 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/model/diagnostic_filter_emergency_routing_status.py
--rw-rw-rw-  2.0 fat      617 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/model/diagnostic_filter_packet_type.py
--rw-rw-rw-  2.0 fat      520 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/model/diagnostic_filter_payload_status.py
--rw-rw-rw-  2.0 fat      498 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/model/diagnostic_filter_source.py
--rw-rw-rw-  2.0 fat     3124 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/model/dpri_status.py
--rw-rw-rw-  2.0 fat     1494 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/model/io_buffer.py
--rw-rw-rw-  2.0 fat      772 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/model/machine_dimensions.py
--rw-rw-rw-  2.0 fat      622 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/model/mailbox_command.py
--rw-rw-rw-  2.0 fat     6366 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/model/router_diagnostics.py
--rw-rw-rw-  2.0 fat      579 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/model/run_time_error.py
--rw-rw-rw-  2.0 fat     3070 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/model/version_info.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/model/__init__.py
--rw-rw-rw-  2.0 fat     6068 b- defN 16-Apr-28 07:57 SpiNNMan-2016.001/spinnman/model_binaries/reinjector.aplx
--rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/model_binaries/__init__.py
--rw-rw-rw-  2.0 fat     1640 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/abstract_multi_connection_process.py
--rw-rw-rw-  2.0 fat      636 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/processes/abstract_multi_connection_process_connection_selector.py
--rw-rw-rw-  2.0 fat     1680 b- defN 16-Apr-22 09:44 SpiNNMan-2016.001/spinnman/processes/abstract_process.py
--rw-rw-rw-  2.0 fat     1060 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/abstract_single_connection_process.py
--rw-rw-rw-  2.0 fat      749 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/application_run_process.py
--rw-rw-rw-  2.0 fat     9034 b- defN 16-Apr-20 08:28 SpiNNMan-2016.001/spinnman/processes/check_machine_booted_process.py
--rw-rw-rw-  2.0 fat     1061 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/de_alloc_sdram_process.py
--rw-rw-rw-  2.0 fat      682 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/exit_dpri_process.py
--rw-rw-rw-  2.0 fat     1597 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/get_cpu_info_process.py
--rw-rw-rw-  2.0 fat    10871 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/get_machine_process.py
--rw-rw-rw-  2.0 fat     2244 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/get_routes_process.py
--rw-rw-rw-  2.0 fat     2295 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/get_tags_process.py
--rw-rw-rw-  2.0 fat      803 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/get_version_process.py
--rw-rw-rw-  2.0 fat     3041 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/load_routes_process.py
--rw-rw-rw-  2.0 fat      876 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/malloc_sdram_process.py
--rw-rw-rw-  2.0 fat     1573 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/multi_connection_process_most_direct_connection_selector.py
--rw-rw-rw-  2.0 fat      760 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/multi_connection_process_round_robin_connection_selector.py
--rw-rw-rw-  2.0 fat      778 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/read_dpri_status_process.py
--rw-rw-rw-  2.0 fat     5564 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/read_iobuf_process.py
--rw-rw-rw-  2.0 fat     1941 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/read_memory_process.py
--rw-rw-rw-  2.0 fat     1795 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/read_router_diagnostics_process.py
--rw-rw-rw-  2.0 fat      735 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/reset_dpri_counters_process.py
--rw-rw-rw-  2.0 fat      658 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/send_single_command_process.py
--rw-rw-rw-  2.0 fat      796 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/set_dpri_packet_types_process.py
--rw-rw-rw-  2.0 fat      842 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/set_dpri_router_emergency_timeout_process.py
--rw-rw-rw-  2.0 fat      805 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/set_dpri_router_timeout_process.py
--rw-rw-rw-  2.0 fat     2980 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/write_memory_flood_process.py
--rw-rw-rw-  2.0 fat     3742 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/processes/write_memory_process.py
--rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/processes/__init__.py
--rw-rw-rw-  2.0 fat     1045 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/utilities/locate_connected_machine_ip_address.py
--rw-rw-rw-  2.0 fat     2614 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/utilities/reports.py
--rw-rw-rw-  2.0 fat     9407 b- defN 16-Apr-01 15:00 SpiNNMan-2016.001/spinnman/utilities/utility_functions.py
--rw-rw-rw-  2.0 fat        1 b- defN 15-Dec-08 08:47 SpiNNMan-2016.001/spinnman/utilities/__init__.py
--rw-rw-rw-  2.0 fat        1 b- defN 16-Apr-28 13:51 SpiNNMan-2016.001/SpiNNMan.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat      268 b- defN 16-Apr-28 13:51 SpiNNMan-2016.001/SpiNNMan.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat       36 b- defN 16-Apr-28 13:51 SpiNNMan-2016.001/SpiNNMan.egg-info/requires.txt
--rw-rw-rw-  2.0 fat    14540 b- defN 16-Apr-28 13:51 SpiNNMan-2016.001/SpiNNMan.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        9 b- defN 16-Apr-28 13:51 SpiNNMan-2016.001/SpiNNMan.egg-info/top_level.txt
-245 files, 632166 bytes uncompressed, 176445 bytes compressed:  72.1%
+Zip file size: 229832 bytes, number of entries: 247
+-rw-rw-rw-  2.0 fat      265 b- defN 16-Sep-02 09:01 SpiNNMan-3.0.0/PKG-INFO
+-rw-rw-rw-  2.0 fat     1344 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/README
+-rw-rw-rw-  2.0 fat       64 b- defN 16-Sep-02 09:01 SpiNNMan-3.0.0/setup.cfg
+-rw-rw-rw-  2.0 fat     1720 b- defN 16-Sep-01 19:30 SpiNNMan-3.0.0/setup.py
+-rw-rw-rw-  2.0 fat     5667 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/constants.py
+-rw-rw-rw-  2.0 fat     7813 b- defN 16-Apr-22 09:44 SpiNNMan-3.0.0/spinnman/exceptions.py
+-rw-rw-rw-  2.0 fat   130136 b- defN 16-Sep-01 16:06 SpiNNMan-3.0.0/spinnman/transceiver.py
+-rw-rw-rw-  2.0 fat     5441 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/__init__.py
+-rw-rw-rw-  2.0 fat     1836 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/connections/connection_listener.py
+-rw-rw-rw-  2.0 fat    10185 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/connections/scp_request_pipeline.py
+-rw-rw-rw-  2.0 fat     1123 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/connections/socket_address_with_chip.py
+-rw-rw-rw-  2.0 fat     1644 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/connections/token_bucket.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/connections/__init__.py
+-rw-rw-rw-  2.0 fat      816 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_connection.py
+-rw-rw-rw-  2.0 fat     1450 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_eieio_receiver.py
+-rw-rw-rw-  2.0 fat      761 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_eieio_sender.py
+-rw-rw-rw-  2.0 fat      656 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_listenable.py
+-rw-rw-rw-  2.0 fat     1903 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_multicast_receiver.py
+-rw-rw-rw-  2.0 fat     1275 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_multicast_sender.py
+-rw-rw-rw-  2.0 fat     1681 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_scp_receiver.py
+-rw-rw-rw-  2.0 fat     1826 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_scp_sender.py
+-rw-rw-rw-  2.0 fat     1385 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_sdp_receiver.py
+-rw-rw-rw-  2.0 fat      729 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_sdp_sender.py
+-rw-rw-rw-  2.0 fat     1482 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_spinnaker_boot_receiver.py
+-rw-rw-rw-  2.0 fat      839 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_spinnaker_boot_sender.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/connections/abstract_classes/__init__.py
+-rw-rw-rw-  2.0 fat     3348 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_bmp_connection.py
+-rw-rw-rw-  2.0 fat     2749 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_boot_connection.py
+-rw-rw-rw-  2.0 fat     9565 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_connection.py
+-rw-rw-rw-  2.0 fat     2452 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_eieio_connection.py
+-rw-rw-rw-  2.0 fat     1073 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_ip_address_connection.py
+-rw-rw-rw-  2.0 fat     2810 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_scamp_connection.py
+-rw-rw-rw-  2.0 fat     3045 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_sdp_connection.py
+-rw-rw-rw-  2.0 fat      615 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_utils.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/__init__.py
+-rw-rw-rw-  2.0 fat      800 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/multicast_message.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/__init__.py
+-rw-rw-rw-  2.0 fat     3902 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/create_eieio_command.py
+-rw-rw-rw-  2.0 fat    16418 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/create_eieio_data.py
+-rw-rw-rw-  2.0 fat      458 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/eieio/eieio_prefix.py
+-rw-rw-rw-  2.0 fat     1316 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/eieio/eieio_type.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/eieio/__init__.py
+-rw-rw-rw-  2.0 fat      170 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/eieio/abstract_messages/abstract_eieio_message.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/eieio/abstract_messages/__init__.py
+-rw-rw-rw-  2.0 fat     1207 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/database_confirmation.py
+-rw-rw-rw-  2.0 fat     1593 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/eieio_command_header.py
+-rw-rw-rw-  2.0 fat     1537 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/eieio_command_message.py
+-rw-rw-rw-  2.0 fat      581 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/event_stop_request.py
+-rw-rw-rw-  2.0 fat     5604 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/host_data_read.py
+-rw-rw-rw-  2.0 fat     1781 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/host_send_sequenced_data.py
+-rw-rw-rw-  2.0 fat      583 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/padding_request.py
+-rw-rw-rw-  2.0 fat     1977 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/spinnaker_request_buffers.py
+-rw-rw-rw-  2.0 fat     8225 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/spinnaker_request_read_data.py
+-rw-rw-rw-  2.0 fat      662 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/start_requests.py
+-rw-rw-rw-  2.0 fat      636 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/stop_requests.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/__init__.py
+-rw-rw-rw-  2.0 fat      720 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/abstract_eieio_data_element.py
+-rw-rw-rw-  2.0 fat     8094 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_data_header.py
+-rw-rw-rw-  2.0 fat     6851 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_data_message.py
+-rw-rw-rw-  2.0 fat     1210 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_key_data_element.py
+-rw-rw-rw-  2.0 fat     1648 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_key_payload_data_element.py
+-rw-rw-rw-  2.0 fat     1338 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_without_payload_data_message.py
+-rw-rw-rw-  2.0 fat     1844 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_with_payload_data_message.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/__init__.py
+-rw-rw-rw-  2.0 fat      802 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_data_message.py
+-rw-rw-rw-  2.0 fat      977 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_lower_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat      949 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_payload_prefix_data_message.py
+-rw-rw-rw-  2.0 fat     1136 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_payload_prefix_lower_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat     1306 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_payload_prefix_upper_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat      979 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_timed_payload_prefix_data_message.py
+-rw-rw-rw-  2.0 fat     1139 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_timed_payload_prefix_lower_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat     1275 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_timed_payload_prefix_upper_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat     1162 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_upper_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/__init__.py
+-rw-rw-rw-  2.0 fat      865 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_data_message.py
+-rw-rw-rw-  2.0 fat     1015 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_lower_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat     1033 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_payload_prefix_data_message.py
+-rw-rw-rw-  2.0 fat     1162 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_payload_prefix_lower_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat     1299 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_payload_prefix_upper_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat      959 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_timed_data_message.py
+-rw-rw-rw-  2.0 fat     1136 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_timed_lower_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat     1272 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_timed_upper_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat     1186 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_upper_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/__init__.py
+-rw-rw-rw-  2.0 fat      801 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_data_message.py
+-rw-rw-rw-  2.0 fat      977 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_lower_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat      949 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_payload_prefix_data_message.py
+-rw-rw-rw-  2.0 fat     1137 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_payload_prefix_lower_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat     1305 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_payload_prefix_upper_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat     1012 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_timed_payload_prefix_data_message.py
+-rw-rw-rw-  2.0 fat     1172 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_timed_payload_prefix_lower_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat     1274 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_timed_payload_prefix_upper_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat     1113 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_upper_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/__init__.py
+-rw-rw-rw-  2.0 fat      830 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_data_message.py
+-rw-rw-rw-  2.0 fat     1015 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_lower_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat     1033 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_payload_prefix_data_message.py
+-rw-rw-rw-  2.0 fat     1162 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_payload_prefix_lower_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat     1298 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_payload_prefix_upper_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat      946 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_timed_data_message.py
+-rw-rw-rw-  2.0 fat     1135 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_timed_lower_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat     1271 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_timed_upper_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat     1185 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_upper_key_prefix_data_message.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/__init__.py
+-rw-rw-rw-  2.0 fat      664 b- defN 16-Jan-18 10:20 SpiNNMan-3.0.0/spinnman/messages/scp/scp_alloc_free_type.py
+-rw-rw-rw-  2.0 fat      465 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/scp/scp_bmp_info_type.py
+-rw-rw-rw-  2.0 fat     1317 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/messages/scp/scp_command.py
+-rw-rw-rw-  2.0 fat      683 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/scp/scp_dpri_command.py
+-rw-rw-rw-  2.0 fat      427 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/scp/scp_dpri_packet_type_flags.py
+-rw-rw-rw-  2.0 fat      363 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/scp/scp_iptag_command.py
+-rw-rw-rw-  2.0 fat      410 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/scp/scp_led_action.py
+-rw-rw-rw-  2.0 fat      396 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/scp/scp_power_command.py
+-rw-rw-rw-  2.0 fat     2013 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/scp/scp_request_header.py
+-rw-rw-rw-  2.0 fat     1095 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/scp/scp_response_header.py
+-rw-rw-rw-  2.0 fat     1002 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/scp/scp_result.py
+-rw-rw-rw-  2.0 fat     1385 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/messages/scp/scp_signal.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/__init__.py
+-rw-rw-rw-  2.0 fat      355 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/abstract_messages/abstract_scp_bmp_reponse.py
+-rw-rw-rw-  2.0 fat     1771 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/abstract_messages/abstract_scp_bmp_request.py
+-rw-rw-rw-  2.0 fat     3759 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/messages/scp/abstract_messages/abstract_scp_request.py
+-rw-rw-rw-  2.0 fat     2218 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/abstract_messages/abstract_scp_response.py
+-rw-rw-rw-  2.0 fat       24 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/abstract_messages/__init__.py
+-rw-rw-rw-  2.0 fat     1795 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_application_run_request.py
+-rw-rw-rw-  2.0 fat     1575 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_app_stop_request.py
+-rw-rw-rw-  2.0 fat     1793 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_bmp_set_led_request.py
+-rw-rw-rw-  2.0 fat     1142 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_bmp_version_request.py
+-rw-rw-rw-  2.0 fat     1103 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_check_ok_response.py
+-rw-rw-rw-  2.0 fat     1670 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_chip_info_request.py
+-rw-rw-rw-  2.0 fat     1279 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_chip_info_response.py
+-rw-rw-rw-  2.0 fat     1659 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_count_state_request.py
+-rw-rw-rw-  2.0 fat     1130 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_count_state_response.py
+-rw-rw-rw-  2.0 fat     1454 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_dpri_exit_request.py
+-rw-rw-rw-  2.0 fat     1415 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_dpri_get_status_request.py
+-rw-rw-rw-  2.0 fat     1169 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_dpri_get_status_response.py
+-rw-rw-rw-  2.0 fat     1520 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_dpri_reset_counters_request.py
+-rw-rw-rw-  2.0 fat     1948 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_dpri_set_reinjection_packet_types.py
+-rw-rw-rw-  2.0 fat     1919 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_dpri_set_router_emergency_timeout_request.py
+-rw-rw-rw-  2.0 fat     1835 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_dpri_set_router_timeout_request.py
+-rw-rw-rw-  2.0 fat     2294 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_flood_fill_data_request.py
+-rw-rw-rw-  2.0 fat     2021 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_flood_fill_end_request.py
+-rw-rw-rw-  2.0 fat     2160 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_flood_fill_start_request.py
+-rw-rw-rw-  2.0 fat     1270 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_iptag_clear_request.py
+-rw-rw-rw-  2.0 fat     1350 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_iptag_get_request.py
+-rw-rw-rw-  2.0 fat     4192 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_iptag_get_response.py
+-rw-rw-rw-  2.0 fat     1226 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_iptag_info_request.py
+-rw-rw-rw-  2.0 fat     1563 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_iptag_info_response.py
+-rw-rw-rw-  2.0 fat     1778 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_iptag_set_request.py
+-rw-rw-rw-  2.0 fat     1521 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_iptag_tto_request.py
+-rw-rw-rw-  2.0 fat     1705 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_led_request.py
+-rw-rw-rw-  2.0 fat     1477 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_power_request.py
+-rw-rw-rw-  2.0 fat      959 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_adc_request.py
+-rw-rw-rw-  2.0 fat     1060 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_adc_response.py
+-rw-rw-rw-  2.0 fat     1421 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_fpga_register_request.py
+-rw-rw-rw-  2.0 fat     1189 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_fpga_register_response.py
+-rw-rw-rw-  2.0 fat     1838 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_link_request.py
+-rw-rw-rw-  2.0 fat     1465 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_link_response.py
+-rw-rw-rw-  2.0 fat     1969 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_memory_request.py
+-rw-rw-rw-  2.0 fat     1312 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_memory_response.py
+-rw-rw-rw-  2.0 fat     2179 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_reverse_iptag_set_request.py
+-rw-rw-rw-  2.0 fat     1657 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_router_alloc_request.py
+-rw-rw-rw-  2.0 fat     1134 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_router_alloc_response.py
+-rw-rw-rw-  2.0 fat     1405 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_router_clear_request.py
+-rw-rw-rw-  2.0 fat     2791 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_router_init_request.py
+-rw-rw-rw-  2.0 fat     2266 b- defN 16-Apr-19 14:13 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_sdram_alloc_request.py
+-rw-rw-rw-  2.0 fat     1598 b- defN 16-Apr-19 14:14 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_sdram_alloc_response.py
+-rw-rw-rw-  2.0 fat     2397 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_sdram_de_alloc_request.py
+-rw-rw-rw-  2.0 fat     1561 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_sdram_de_alloc_response.py
+-rw-rw-rw-  2.0 fat     1883 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_send_signal_request.py
+-rw-rw-rw-  2.0 fat     1603 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_version_request.py
+-rw-rw-rw-  2.0 fat     1185 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_version_response.py
+-rw-rw-rw-  2.0 fat     1749 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_write_fpga_register_request.py
+-rw-rw-rw-  2.0 fat     2063 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_write_link_request.py
+-rw-rw-rw-  2.0 fat     2037 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_write_memory_request.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:46 SpiNNMan-3.0.0/spinnman/messages/scp/impl/__init__.py
+-rw-rw-rw-  2.0 fat      448 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/sdp/sdp_flag.py
+-rw-rw-rw-  2.0 fat     9257 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/messages/sdp/sdp_header.py
+-rw-rw-rw-  2.0 fat     1735 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/sdp/sdp_message.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/sdp/__init__.py
+-rw-rw-rw-  2.0 fat     3242 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/spinnaker_boot/spinnaker_boot_message.py
+-rw-rw-rw-  2.0 fat     5670 b- defN 16-Aug-24 20:46 SpiNNMan-3.0.0/spinnman/messages/spinnaker_boot/spinnaker_boot_messages.py
+-rw-rw-rw-  2.0 fat      430 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/spinnaker_boot/spinnaker_boot_op_code.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/spinnaker_boot/__init__.py
+-rw-rw-rw-  2.0 fat    27068 b- defN 16-Sep-01 07:50 SpiNNMan-3.0.0/spinnman/messages/spinnaker_boot/boot_data/scamp-3.boot
+-rw-rw-rw-  2.0 fat    14500 b- defN 16-Jul-11 14:39 SpiNNMan-3.0.0/spinnman/messages/spinnaker_boot/_system_variables/_system_variable_boot_values.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/messages/spinnaker_boot/_system_variables/__init__.py
+-rw-rw-rw-  2.0 fat     3767 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/model/adc_info.py
+-rw-rw-rw-  2.0 fat     1306 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/model/bmp_connection_data.py
+-rw-rw-rw-  2.0 fat     6572 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/model/chip_info.py
+-rw-rw-rw-  2.0 fat     4260 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/model/chip_summary_info.py
+-rw-rw-rw-  2.0 fat     7972 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/model/cpu_info.py
+-rw-rw-rw-  2.0 fat      587 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/model/cpu_state.py
+-rw-rw-rw-  2.0 fat     9054 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/model/diagnostic_filter.py
+-rw-rw-rw-  2.0 fat      555 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/model/diagnostic_filter_default_routing_status.py
+-rw-rw-rw-  2.0 fat      859 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/model/diagnostic_filter_destination.py
+-rw-rw-rw-  2.0 fat     1011 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/model/diagnostic_filter_emergency_routing_status.py
+-rw-rw-rw-  2.0 fat      617 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/model/diagnostic_filter_packet_type.py
+-rw-rw-rw-  2.0 fat      520 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/model/diagnostic_filter_payload_status.py
+-rw-rw-rw-  2.0 fat      498 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/model/diagnostic_filter_source.py
+-rw-rw-rw-  2.0 fat     3124 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/model/dpri_status.py
+-rw-rw-rw-  2.0 fat     1494 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/model/io_buffer.py
+-rw-rw-rw-  2.0 fat      772 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/model/machine_dimensions.py
+-rw-rw-rw-  2.0 fat      622 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/model/mailbox_command.py
+-rw-rw-rw-  2.0 fat     2476 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/model/p2p_table.py
+-rw-rw-rw-  2.0 fat      533 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/model/p2p_table_route.py
+-rw-rw-rw-  2.0 fat     6366 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/model/router_diagnostics.py
+-rw-rw-rw-  2.0 fat      612 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/model/run_time_error.py
+-rw-rw-rw-  2.0 fat     3777 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/model/version_info.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/model/__init__.py
+-rw-rw-rw-  2.0 fat     4852 b- defN 16-Sep-02 09:00 SpiNNMan-3.0.0/spinnman/model_binaries/reinjector.aplx
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/model_binaries/__init__.py
+-rw-rw-rw-  2.0 fat     1640 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/abstract_multi_connection_process.py
+-rw-rw-rw-  2.0 fat      636 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/processes/abstract_multi_connection_process_connection_selector.py
+-rw-rw-rw-  2.0 fat     1680 b- defN 16-Apr-22 09:44 SpiNNMan-3.0.0/spinnman/processes/abstract_process.py
+-rw-rw-rw-  2.0 fat     1060 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/abstract_single_connection_process.py
+-rw-rw-rw-  2.0 fat      749 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/application_run_process.py
+-rw-rw-rw-  2.0 fat     1061 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/de_alloc_sdram_process.py
+-rw-rw-rw-  2.0 fat      682 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/exit_dpri_process.py
+-rw-rw-rw-  2.0 fat     1663 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/processes/get_cpu_info_process.py
+-rw-rw-rw-  2.0 fat     7517 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/processes/get_machine_process.py
+-rw-rw-rw-  2.0 fat     2244 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/get_routes_process.py
+-rw-rw-rw-  2.0 fat     2295 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/get_tags_process.py
+-rw-rw-rw-  2.0 fat      803 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/get_version_process.py
+-rw-rw-rw-  2.0 fat     3041 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/load_routes_process.py
+-rw-rw-rw-  2.0 fat      876 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/malloc_sdram_process.py
+-rw-rw-rw-  2.0 fat     1573 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/multi_connection_process_most_direct_connection_selector.py
+-rw-rw-rw-  2.0 fat      760 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/multi_connection_process_round_robin_connection_selector.py
+-rw-rw-rw-  2.0 fat      778 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/read_dpri_status_process.py
+-rw-rw-rw-  2.0 fat     5945 b- defN 16-Sep-01 07:50 SpiNNMan-3.0.0/spinnman/processes/read_iobuf_process.py
+-rw-rw-rw-  2.0 fat     1941 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/read_memory_process.py
+-rw-rw-rw-  2.0 fat     1795 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/read_router_diagnostics_process.py
+-rw-rw-rw-  2.0 fat      735 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/reset_dpri_counters_process.py
+-rw-rw-rw-  2.0 fat      658 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/send_single_command_process.py
+-rw-rw-rw-  2.0 fat      796 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/set_dpri_packet_types_process.py
+-rw-rw-rw-  2.0 fat      842 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/set_dpri_router_emergency_timeout_process.py
+-rw-rw-rw-  2.0 fat      805 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/set_dpri_router_timeout_process.py
+-rw-rw-rw-  2.0 fat     2980 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/write_memory_flood_process.py
+-rw-rw-rw-  2.0 fat     3742 b- defN 16-Apr-01 15:00 SpiNNMan-3.0.0/spinnman/processes/write_memory_process.py
+-rw-rw-rw-  2.0 fat        0 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/processes/__init__.py
+-rw-rw-rw-  2.0 fat     1045 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/utilities/locate_connected_machine_ip_address.py
+-rw-rw-rw-  2.0 fat     2614 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/utilities/reports.py
+-rw-rw-rw-  2.0 fat     2808 b- defN 16-Jul-11 11:49 SpiNNMan-3.0.0/spinnman/utilities/utility_functions.py
+-rw-rw-rw-  2.0 fat        1 b- defN 15-Dec-08 08:47 SpiNNMan-3.0.0/spinnman/utilities/__init__.py
+-rw-rw-rw-  2.0 fat        1 b- defN 16-Sep-02 09:01 SpiNNMan-3.0.0/SpiNNMan.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat      265 b- defN 16-Sep-02 09:01 SpiNNMan-3.0.0/SpiNNMan.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat       80 b- defN 16-Sep-02 09:01 SpiNNMan-3.0.0/SpiNNMan.egg-info/requires.txt
+-rw-rw-rw-  2.0 fat    14629 b- defN 16-Sep-02 09:01 SpiNNMan-3.0.0/SpiNNMan.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 16-Sep-02 09:01 SpiNNMan-3.0.0/SpiNNMan.egg-info/top_level.txt
+247 files, 615456 bytes uncompressed, 174824 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -1,736 +1,742 @@
-Filename: SpiNNMan-2016.001/PKG-INFO
+Filename: SpiNNMan-3.0.0/PKG-INFO
 Comment: 
 
-Filename: SpiNNMan-2016.001/README
+Filename: SpiNNMan-3.0.0/README
 Comment: 
 
-Filename: SpiNNMan-2016.001/setup.cfg
+Filename: SpiNNMan-3.0.0/setup.cfg
 Comment: 
 
-Filename: SpiNNMan-2016.001/setup.py
+Filename: SpiNNMan-3.0.0/setup.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/constants.py
+Filename: SpiNNMan-3.0.0/spinnman/constants.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/exceptions.py
+Filename: SpiNNMan-3.0.0/spinnman/exceptions.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/transceiver.py
+Filename: SpiNNMan-3.0.0/spinnman/transceiver.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/connection_listener.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/connection_listener.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/scp_request_pipeline.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/scp_request_pipeline.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/socket_address_with_chip.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/socket_address_with_chip.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/token_bucket.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/token_bucket.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_connection.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_connection.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_eieio_receiver.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_eieio_receiver.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_eieio_sender.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_eieio_sender.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_listenable.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_listenable.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_multicast_receiver.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_multicast_receiver.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_multicast_sender.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_multicast_sender.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_scp_receiver.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_scp_receiver.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_scp_sender.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_scp_sender.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_sdp_receiver.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_sdp_receiver.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_sdp_sender.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_sdp_sender.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_spinnaker_boot_receiver.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_spinnaker_boot_receiver.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_spinnaker_boot_sender.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_spinnaker_boot_sender.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/abstract_classes/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/abstract_classes/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_bmp_connection.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_bmp_connection.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_boot_connection.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_boot_connection.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_connection.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_connection.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_eieio_connection.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_eieio_connection.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_ip_address_connection.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_ip_address_connection.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_scamp_connection.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_scamp_connection.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_sdp_connection.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_sdp_connection.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_utils.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_utils.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/multicast_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/multicast_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/create_eieio_command.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/create_eieio_command.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/create_eieio_data.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/create_eieio_data.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/eieio_prefix.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/eieio_prefix.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/eieio_type.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/eieio_type.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/abstract_messages/abstract_eieio_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/abstract_messages/abstract_eieio_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/abstract_messages/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/abstract_messages/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/database_confirmation.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/database_confirmation.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/eieio_command_header.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/eieio_command_header.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/eieio_command_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/eieio_command_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/event_stop_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/event_stop_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/host_data_read.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/host_data_read.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/host_send_sequenced_data.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/host_send_sequenced_data.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/padding_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/padding_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/spinnaker_request_buffers.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/spinnaker_request_buffers.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/spinnaker_request_read_data.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/spinnaker_request_read_data.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/start_requests.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/start_requests.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/stop_requests.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/stop_requests.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/abstract_eieio_data_element.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/abstract_eieio_data_element.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_data_header.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_data_header.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_key_data_element.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_key_data_element.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_key_payload_data_element.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_key_payload_data_element.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_without_payload_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_without_payload_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_with_payload_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_with_payload_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_lower_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_lower_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_payload_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_payload_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_payload_prefix_lower_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_payload_prefix_lower_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_payload_prefix_upper_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_payload_prefix_upper_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_timed_payload_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_timed_payload_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_timed_payload_prefix_lower_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_timed_payload_prefix_lower_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_timed_payload_prefix_upper_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_timed_payload_prefix_upper_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_upper_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_upper_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_lower_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_lower_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_payload_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_payload_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_payload_prefix_lower_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_payload_prefix_lower_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_payload_prefix_upper_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_payload_prefix_upper_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_timed_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_timed_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_timed_lower_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_timed_lower_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_timed_upper_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_timed_upper_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_upper_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_upper_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_lower_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_lower_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_payload_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_payload_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_payload_prefix_lower_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_payload_prefix_lower_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_payload_prefix_upper_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_payload_prefix_upper_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_timed_payload_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_timed_payload_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_timed_payload_prefix_lower_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_timed_payload_prefix_lower_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_timed_payload_prefix_upper_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_timed_payload_prefix_upper_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_upper_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_upper_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_lower_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_lower_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_payload_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_payload_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_payload_prefix_lower_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_payload_prefix_lower_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_payload_prefix_upper_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_payload_prefix_upper_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_timed_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_timed_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_timed_lower_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_timed_lower_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_timed_upper_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_timed_upper_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_upper_key_prefix_data_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_upper_key_prefix_data_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/scp_alloc_free_type.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/scp_alloc_free_type.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/scp_bmp_info_type.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/scp_bmp_info_type.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/scp_command.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/scp_command.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/scp_dpri_command.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/scp_dpri_command.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/scp_dpri_packet_type_flags.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/scp_dpri_packet_type_flags.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/scp_iptag_command.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/scp_iptag_command.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/scp_led_action.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/scp_led_action.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/scp_power_command.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/scp_power_command.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/scp_request_header.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/scp_request_header.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/scp_response_header.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/scp_response_header.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/scp_result.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/scp_result.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/scp_signal.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/scp_signal.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/abstract_messages/abstract_scp_bmp_reponse.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/abstract_messages/abstract_scp_bmp_reponse.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/abstract_messages/abstract_scp_bmp_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/abstract_messages/abstract_scp_bmp_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/abstract_messages/abstract_scp_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/abstract_messages/abstract_scp_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/abstract_messages/abstract_scp_response.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/abstract_messages/abstract_scp_response.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/abstract_messages/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/abstract_messages/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_application_run_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_application_run_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_app_stop_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_app_stop_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_bmp_set_led_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_bmp_set_led_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_bmp_version_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_bmp_version_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_check_ok_response.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_check_ok_response.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_count_state_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_chip_info_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_count_state_response.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_chip_info_response.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_dpri_exit_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_count_state_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_dpri_get_status_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_count_state_response.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_dpri_get_status_response.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_dpri_exit_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_dpri_reset_counters_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_dpri_get_status_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_dpri_set_reinjection_packet_types.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_dpri_get_status_response.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_dpri_set_router_emergency_timeout_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_dpri_reset_counters_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_dpri_set_router_timeout_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_dpri_set_reinjection_packet_types.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_flood_fill_data_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_dpri_set_router_emergency_timeout_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_flood_fill_end_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_dpri_set_router_timeout_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_flood_fill_start_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_flood_fill_data_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_iptag_clear_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_flood_fill_end_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_iptag_get_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_flood_fill_start_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_iptag_get_response.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_iptag_clear_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_iptag_info_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_iptag_get_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_iptag_info_response.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_iptag_get_response.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_iptag_set_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_iptag_info_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_iptag_tto_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_iptag_info_response.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_led_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_iptag_set_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_power_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_iptag_tto_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_adc_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_led_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_adc_response.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_power_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_fpga_register_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_adc_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_fpga_register_response.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_adc_response.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_link_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_fpga_register_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_link_response.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_fpga_register_response.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_memory_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_link_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_memory_response.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_link_response.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_reverse_iptag_set_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_memory_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_router_alloc_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_memory_response.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_router_alloc_response.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_reverse_iptag_set_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_router_clear_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_router_alloc_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_router_init_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_router_alloc_response.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_sdram_alloc_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_router_clear_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_sdram_alloc_response.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_router_init_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_sdram_de_alloc_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_sdram_alloc_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_sdram_de_alloc_response.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_sdram_alloc_response.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_send_signal_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_sdram_de_alloc_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_version_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_sdram_de_alloc_response.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_version_response.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_send_signal_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_write_fpga_register_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_version_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_write_link_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_version_response.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_write_memory_request.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_write_fpga_register_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/scp/impl/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_write_link_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/sdp/sdp_flag.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_write_memory_request.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/sdp/sdp_header.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/scp/impl/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/sdp/sdp_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/sdp/sdp_flag.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/sdp/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/sdp/sdp_header.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/spinnaker_boot/spinnaker_boot_message.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/sdp/sdp_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/spinnaker_boot/spinnaker_boot_messages.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/sdp/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/spinnaker_boot/spinnaker_boot_op_code.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/spinnaker_boot/spinnaker_boot_message.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/spinnaker_boot/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/spinnaker_boot/spinnaker_boot_messages.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/spinnaker_boot/boot_data/scamp-133.boot
+Filename: SpiNNMan-3.0.0/spinnman/messages/spinnaker_boot/spinnaker_boot_op_code.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/spinnaker_boot/_system_variables/_system_variable_boot_values.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/spinnaker_boot/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/messages/spinnaker_boot/_system_variables/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/spinnaker_boot/boot_data/scamp-3.boot
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/adc_info.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/spinnaker_boot/_system_variables/_system_variable_boot_values.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/bmp_connection_data.py
+Filename: SpiNNMan-3.0.0/spinnman/messages/spinnaker_boot/_system_variables/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/chip_info.py
+Filename: SpiNNMan-3.0.0/spinnman/model/adc_info.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/core_subset.py
+Filename: SpiNNMan-3.0.0/spinnman/model/bmp_connection_data.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/core_subsets.py
+Filename: SpiNNMan-3.0.0/spinnman/model/chip_info.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/cpu_info.py
+Filename: SpiNNMan-3.0.0/spinnman/model/chip_summary_info.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/cpu_state.py
+Filename: SpiNNMan-3.0.0/spinnman/model/cpu_info.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/diagnostic_filter.py
+Filename: SpiNNMan-3.0.0/spinnman/model/cpu_state.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/diagnostic_filter_default_routing_status.py
+Filename: SpiNNMan-3.0.0/spinnman/model/diagnostic_filter.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/diagnostic_filter_destination.py
+Filename: SpiNNMan-3.0.0/spinnman/model/diagnostic_filter_default_routing_status.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/diagnostic_filter_emergency_routing_status.py
+Filename: SpiNNMan-3.0.0/spinnman/model/diagnostic_filter_destination.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/diagnostic_filter_packet_type.py
+Filename: SpiNNMan-3.0.0/spinnman/model/diagnostic_filter_emergency_routing_status.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/diagnostic_filter_payload_status.py
+Filename: SpiNNMan-3.0.0/spinnman/model/diagnostic_filter_packet_type.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/diagnostic_filter_source.py
+Filename: SpiNNMan-3.0.0/spinnman/model/diagnostic_filter_payload_status.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/dpri_status.py
+Filename: SpiNNMan-3.0.0/spinnman/model/diagnostic_filter_source.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/io_buffer.py
+Filename: SpiNNMan-3.0.0/spinnman/model/dpri_status.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/machine_dimensions.py
+Filename: SpiNNMan-3.0.0/spinnman/model/io_buffer.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/mailbox_command.py
+Filename: SpiNNMan-3.0.0/spinnman/model/machine_dimensions.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/router_diagnostics.py
+Filename: SpiNNMan-3.0.0/spinnman/model/mailbox_command.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/run_time_error.py
+Filename: SpiNNMan-3.0.0/spinnman/model/p2p_table.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/version_info.py
+Filename: SpiNNMan-3.0.0/spinnman/model/p2p_table_route.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/model/router_diagnostics.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model_binaries/reinjector.aplx
+Filename: SpiNNMan-3.0.0/spinnman/model/run_time_error.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/model_binaries/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/model/version_info.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/abstract_multi_connection_process.py
+Filename: SpiNNMan-3.0.0/spinnman/model/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/abstract_multi_connection_process_connection_selector.py
+Filename: SpiNNMan-3.0.0/spinnman/model_binaries/reinjector.aplx
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/abstract_process.py
+Filename: SpiNNMan-3.0.0/spinnman/model_binaries/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/abstract_single_connection_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/abstract_multi_connection_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/application_run_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/abstract_multi_connection_process_connection_selector.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/check_machine_booted_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/abstract_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/de_alloc_sdram_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/abstract_single_connection_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/exit_dpri_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/application_run_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/get_cpu_info_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/de_alloc_sdram_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/get_machine_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/exit_dpri_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/get_routes_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/get_cpu_info_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/get_tags_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/get_machine_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/get_version_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/get_routes_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/load_routes_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/get_tags_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/malloc_sdram_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/get_version_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/multi_connection_process_most_direct_connection_selector.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/load_routes_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/multi_connection_process_round_robin_connection_selector.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/malloc_sdram_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/read_dpri_status_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/multi_connection_process_most_direct_connection_selector.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/read_iobuf_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/multi_connection_process_round_robin_connection_selector.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/read_memory_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/read_dpri_status_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/read_router_diagnostics_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/read_iobuf_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/reset_dpri_counters_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/read_memory_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/send_single_command_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/read_router_diagnostics_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/set_dpri_packet_types_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/reset_dpri_counters_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/set_dpri_router_emergency_timeout_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/send_single_command_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/set_dpri_router_timeout_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/set_dpri_packet_types_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/write_memory_flood_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/set_dpri_router_emergency_timeout_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/write_memory_process.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/set_dpri_router_timeout_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/processes/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/write_memory_flood_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/utilities/locate_connected_machine_ip_address.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/write_memory_process.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/utilities/reports.py
+Filename: SpiNNMan-3.0.0/spinnman/processes/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/utilities/utility_functions.py
+Filename: SpiNNMan-3.0.0/spinnman/utilities/locate_connected_machine_ip_address.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/spinnman/utilities/__init__.py
+Filename: SpiNNMan-3.0.0/spinnman/utilities/reports.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/SpiNNMan.egg-info/dependency_links.txt
+Filename: SpiNNMan-3.0.0/spinnman/utilities/utility_functions.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/SpiNNMan.egg-info/PKG-INFO
+Filename: SpiNNMan-3.0.0/spinnman/utilities/__init__.py
 Comment: 
 
-Filename: SpiNNMan-2016.001/SpiNNMan.egg-info/requires.txt
+Filename: SpiNNMan-3.0.0/SpiNNMan.egg-info/dependency_links.txt
 Comment: 
 
-Filename: SpiNNMan-2016.001/SpiNNMan.egg-info/SOURCES.txt
+Filename: SpiNNMan-3.0.0/SpiNNMan.egg-info/PKG-INFO
 Comment: 
 
-Filename: SpiNNMan-2016.001/SpiNNMan.egg-info/top_level.txt
+Filename: SpiNNMan-3.0.0/SpiNNMan.egg-info/requires.txt
+Comment: 
+
+Filename: SpiNNMan-3.0.0/SpiNNMan.egg-info/SOURCES.txt
+Comment: 
+
+Filename: SpiNNMan-3.0.0/SpiNNMan.egg-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `SpiNNMan-2016.001/README` & `SpiNNMan-3.0.0/README`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/setup.py` & `SpiNNMan-3.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 setup(
     name="SpiNNMan",
-    version="2016.001",
+    version="3.0.0",
     description="Interaction with a SpiNNaker Machine",
     url="https://github.com/SpiNNakerManchester/SpiNNMan",
     license="GNU GPLv3.0",
     packages=['spinnman',
               'spinnman.connections',
               'spinnman.connections.abstract_classes',
               'spinnman.connections.udp_packet_connections',
@@ -30,9 +30,11 @@
               'spinnman.messages.spinnaker_boot._system_variables',
               'spinnman.model',
               'spinnman.model_binaries',
               'spinnman.processes',
               'spinnman.utilities'],
     package_data={'spinnman.messages.spinnaker_boot': ['boot_data/*.boot'],
                   'spinnman.model_binaries': ['*.aplx']},
-    install_requires=['six', 'enum34', 'SpiNNMachine == 2016.001']
+    install_requires=[
+        'six', 'enum34', 'SpiNNMachine >= 3.0.0, < 4.0.0',
+        'SpiNNStorageHandlers >= 3.0.0, < 4.0.0']
 )
```

## Comparing `SpiNNMan-2016.001/spinnman/constants.py` & `SpiNNMan-3.0.0/spinnman/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 # The base address of the system variable structure in System ram
 SYSTEM_VARIABLE_BASE_ADDRESS = 0xf5007f00
 
 # The base address of a routers diagnostic filter controls
 ROUTER_REGISTER_BASE_ADDRESS = 0xe1000000
 
+# The base address of a routers p2p routing table
+ROUTER_REGISTER_P2P_ADDRESS = ROUTER_REGISTER_BASE_ADDRESS + 0x10000
+
 # offset for the router filter controls first register (one word each)
 ROUTER_FILTER_CONTROLS_OFFSET = 0x200
 
 # point where default filters finish and user set-able ones are available
 ROUTER_DEFAULT_FILTERS_MAX_POSITION = 11
 
 # size of a router diagnostic filter control register in bytes
@@ -32,26 +35,32 @@
 
 # the amount of size in bytes that the EIEIO command header is
 EIEIO_COMMAND_HEADER_SIZE = 3
 
 # The amount of size in bytes the EIEIO data header is
 EIEIO_DATA_HEADER_SIZE = 2
 
+# the address of the start of the VCPU structure (copied from sark.h)
+CPU_INFO_OFFSET = 0xe5007000
+
 # how many bytes the cpu info data takes up
 CPU_INFO_BYTES = 128
 
 # the address at which user0 register starts
 CPU_USER_0_START_ADDRESS = 112
 
 # the address at which user0 register starts
 CPU_USER_1_START_ADDRESS = 116
 
 # the address at which user0 register starts
 CPU_USER_2_START_ADDRESS = 120
 
+# the address at which the iobuf address starts
+CPU_IOBUF_ADDRESS_OFFSET = 88
+
 # default UDP tag
 DEFAULT_SDP_TAG = 0xFF
 
 # max user requested tag value
 MAX_TAG_ID = 7
 
 # The range of values the BMP's 12-bit ADCs can measure.
```

## Comparing `SpiNNMan-2016.001/spinnman/exceptions.py` & `SpiNNMan-3.0.0/spinnman/exceptions.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/transceiver.py` & `SpiNNMan-3.0.0/spinnman/transceiver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
 # local imports
 from spinnman.connections.udp_packet_connections.udp_bmp_connection import \
     UDPBMPConnection
+from spinnman.messages.scp.abstract_messages.abstract_scp_request import \
+    AbstractSCPRequest
 from spinnman.messages.scp.impl.scp_bmp_set_led_request import \
     SCPBMPSetLedRequest
 from spinnman.messages.scp.impl.scp_bmp_version_request import \
     SCPBMPVersionRequest
 from spinnman.messages.scp.impl.scp_power_request import SCPPowerRequest
 from spinnman.messages.scp.impl.scp_read_adc_request import SCPReadADCRequest
 from spinnman.messages.scp.impl.scp_read_fpga_register_request import \
@@ -35,17 +37,16 @@
 from spinnman.processes.read_memory_process import ReadMemoryProcess
 from spinnman.messages.scp.impl.scp_iptag_tto_request import SCPIPTagTTORequest
 from spinnman.processes.get_cpu_info_process import GetCPUInfoProcess
 from spinnman.processes.read_iobuf_process import ReadIOBufProcess
 from spinnman.processes.application_run_process import ApplicationRunProcess
 from spinnman import model_binaries
 from spinnman.processes.exit_dpri_process import ExitDPRIProcess
-from spinn_machine.utilities import utilities
-from spinnman.processes.check_machine_booted_process \
-    import CheckMachineBootedProcess
+from spinnman.messages.spinnaker_boot._system_variables\
+    ._system_variable_boot_values import SystemVariableDefinition
 from spinnman.processes.set_dpri_packet_types_process \
     import SetDPRIPacketTypesProcess
 from spinnman.messages.scp.scp_dpri_packet_type_flags \
     import SCPDPRIPacketTypeFlags
 from spinnman.processes.set_dpri_router_timeout_process \
     import SetDPRIRouterTimeoutProcess
 from spinnman.processes.set_dpri_router_emergency_timeout_process \
@@ -73,15 +74,14 @@
     import UDPBootConnection
 from spinnman import constants
 from spinnman.connections.udp_packet_connections.udp_scamp_connection \
     import UDPSCAMPConnection
 from spinnman.messages.scp.impl.scp_reverse_iptag_set_request import \
     SCPReverseIPTagSetRequest
 from spinnman.model.machine_dimensions import MachineDimensions
-from spinnman.model.core_subsets import CoreSubsets
 from spinnman.messages.spinnaker_boot.spinnaker_boot_messages \
     import SpinnakerBootMessages
 from spinnman.messages.scp.impl.scp_read_memory_request \
     import SCPReadMemoryRequest
 from spinnman.messages.scp.impl.scp_count_state_request \
     import SCPCountStateRequest
 from spinnman.messages.scp.impl.scp_write_memory_request \
@@ -98,35 +98,39 @@
     import SCPRouterClearRequest
 from spinnman.messages.scp.impl.scp_led_request \
     import SCPLEDRequest
 from spinnman.messages.scp.impl.scp_app_stop_request import SCPAppStopRequest
 from spinnman.utilities import utility_functions
 from spinnman import exceptions
 
+# storage handlers imports
 from spinn_storage_handlers.abstract_classes.abstract_data_reader \
     import AbstractDataReader
 from spinn_storage_handlers.file_data_reader import FileDataReader
 
+# spinnmachine imports
+from spinn_machine.core_subsets import CoreSubsets
+
 # general imports
 import random
 import struct
 from threading import Condition
 from collections import defaultdict
 import logging
 import socket
 import time
 import os
 
 logger = logging.getLogger(__name__)
 
 _SCAMP_NAME = "SC&MP"
-_SCAMP_VERSION = 1.33
+_SCAMP_VERSION = (3, 0, 1)
 
 _BMP_NAME = "BC&MP"
-_BMP_VERSIONS = [1.3, 1.33, 1.37, 1.36]
+_BMP_MAJOR_VERSIONS = [1, 2]
 
 _STANDARD_RETIRES_NO = 3
 INITIAL_FIND_SCAMP_RETRIES_COUNT = 3
 _REINJECTOR_APP_ID = 17
 
 
 def create_transceiver_from_hostname(
@@ -146,19 +150,19 @@
     :param number_of_boards: a number of boards expected to be supported, or\
                 None, which defaults to a single board
     :type number_of_boards: int or None
     :param ignore_chips: An optional set of chips to ignore in the\
                 machine.  Requests for a "machine" will have these chips\
                 excluded, as if they never existed.  The processor_ids of\
                 the specified chips are ignored.
-    :type ignore_chips: :py:class:`spinnman.model.core_subsets.CoreSubsets`
+    :type ignore_chips: :py:class:`spinn_machine.core_subsets.CoreSubsets`
     :param ignore_cores: An optional set of cores to ignore in the\
                 machine.  Requests for a "machine" will have these cores\
                 excluded, as if they never existed.
-    :type ignore_cores: :py:class:`spinnman.model.core_subsets.CoreSubsets`
+    :type ignore_cores: :py:class:`spinn_machine.core_subsets.CoreSubsets`
     :param max_core_id: The maximum core id in any discovered machine.\
                 Requests for a "machine" will only have core ids up to\
                 this value.
     :type max_core_id: int
     :param version: the type of spinnaker board used within the spinnaker\
                 machine being used. If a spinn-5 board, then the version\
                 will be 5, spinn-3 would equal 3 and so on.
@@ -252,19 +256,19 @@
                     connections are found.
         :type connections: iterable of\
                     :py:class:`spinnman.connections.abstract_connection.AbstractConnection`
         :param ignore_chips: An optional set of chips to ignore in the\
                     machine.  Requests for a "machine" will have these chips\
                     excluded, as if they never existed.  The processor_ids of\
                     the specified chips are ignored.
-        :type ignore_chips: :py:class:`spinnman.model.core_subsets.CoreSubsets`
+        :type ignore_chips: :py:class:`spinn_machine.core_subsets.CoreSubsets`
         :param ignore_cores: An optional set of cores to ignore in the\
                     machine.  Requests for a "machine" will have these cores\
                     excluded, as if they never existed.
-        :type ignore_cores: :py:class:`spinnman.model.core_subsets.CoreSubsets`
+        :type ignore_cores: :py:class:`spinn_machine.core_subsets.CoreSubsets`
         :param max_core_id: The maximum core id in any discovered machine.\
                     Requests for a "machine" will only have core ids up to and\
                     including this value.
         :type max_core_id: int
         :param max_sdram_size: the max size each chip can say it has for SDRAM\
                 (mainly used in debugging purposes)
         :type max_sdram_size: int or None
@@ -282,21 +286,21 @@
         :raise spinnman.exceptions.SpinnmanUnexpectedResponseCodeException: If\
                     a response indicates an error during the exchange
         """
 
         # Place to keep the current machine
         self._version = version
         self._machine = None
+        self._width = None
+        self._height = None
         self._ignore_chips = ignore_chips
         self._ignore_cores = ignore_cores
         self._max_core_id = max_core_id
         self._max_sdram_size = max_sdram_size
-
-        # Place to keep the known chip information
-        self._chip_info = dict()
+        self._iobuf_size = None
 
         # Place to keep the identity of the re-injector core on each chip,
         # indexed by chip x and y coordinates
         self._reinjector_cores = CoreSubsets()
         self._reinjection_running = False
 
         # A set of the original connections - used to determine what can
@@ -469,23 +473,28 @@
             try:
                 version_info = self.get_scamp_version(
                     connection.chip_x, connection.chip_y,
                     self._bmp_connection_selectors[(connection.cabinet,
                                                     connection.frame)])
                 fail_version_name = version_info.name != _BMP_NAME
                 fail_version_num = \
-                    version_info.version_number not in _BMP_VERSIONS
+                    version_info.version_number[0] not in _BMP_MAJOR_VERSIONS
                 if fail_version_name or fail_version_num:
                     raise exceptions.SpinnmanIOException(
-                        "The BMP is running {}"
+                        "The BMP at {} is running {}"
                         " {} which is incompatible with this transceiver, "
                         "required version is {} {}".format(
+                            connection.remote_ip_address,
                             version_info.name,
-                            version_info.version_number,
-                            _BMP_NAME, _BMP_VERSIONS))
+                            version_info.version_string,
+                            _BMP_NAME, _BMP_MAJOR_VERSIONS))
+
+                logger.info("Using BMP at {} with version {} {}".format(
+                    connection.remote_ip_address, version_info.name,
+                    version_info.version_string))
 
             # If it fails to respond due to timeout, maybe that the connection
             # isn't valid
             except exceptions.SpinnmanTimeoutException:
                 raise exceptions.SpinnmanException(
                     "BMP connection to {} is not responding".format(
                         connection.remote_ip_address))
@@ -498,14 +507,16 @@
         :return: True if a valid response is received, False otherwise
         """
         current_retries = retries
         while current_retries > 0:
             try:
                 self.get_scamp_version(connection_selector=connection_selector)
                 return True
+            except exceptions.SpinnmanGenericProcessException:
+                current_retries -= 1
             except exceptions.SpinnmanTimeoutException:
                 current_retries -= 1
             except exceptions.SpinnmanUnexpectedResponseCodeException:
                 current_retries -= 1
             except exceptions.SpinnmanIOException:
                 return False
         return False
@@ -661,31 +672,43 @@
         raise exceptions.SpinnmanUnsupportedOperationException(
             "This operation is currently not supported in spinnman.")
 
     def _update_machine(self):
         """ Get the current machine status and store it
         """
 
+        # Get the width and height of the machine
+        self.get_machine_dimensions()
+
+        # Get the coordinates of the boot chip
+        version_info = self.get_scamp_version()
+
         # Get the details of all the chips
         get_machine_process = GetMachineProcess(
             self._scamp_connection_selector, self._ignore_chips,
             self._ignore_cores, self._max_core_id, self._max_sdram_size)
-        self._machine = get_machine_process.get_machine_details()
+        self._machine = get_machine_process.get_machine_details(
+            version_info.x, version_info.y, self._width, self._height)
 
         # update the scamp selector with the machine
         self._scamp_connection_selector.set_machine(self._machine)
 
-        # get cpu information
-        self._chip_info = get_machine_process.get_chip_info()
-
-        # Work out and add the spinnaker links
-        spinnaker_links = utilities.locate_spinnaker_links(
-            self._version, self._machine)
-        for spinnaker_link in spinnaker_links:
-            self._machine.add_spinnaker_link(spinnaker_link)
+        # update the scamp connections replacing any x and y with the default
+        # SCP request params with the boot chip coordinates
+        for connection in self._scamp_connections:
+            if (connection.chip_x ==
+                    AbstractSCPRequest.DEFAULT_DEST_X_COORD) and \
+                    (connection.chip_y ==
+                     AbstractSCPRequest.DEFAULT_DEST_Y_COORD):
+                connection.update_chip_coordinates(
+                    self._machine.boot_x, self._machine.boot_y)
+
+        # Work out and add the spinnaker links and FPGA links
+        self._machine.add_spinnaker_links(self._version)
+        self._machine.add_fpga_links(self._version)
 
         logger.info("Detected a machine on ip address {} which has {}"
                     .format(self._boot_send_connection.remote_ip_address,
                             self._machine.cores_and_link_output_string()))
 
     def discover_scamp_connections(self):
         """ Find connections to the board and store these for future use.\
@@ -707,14 +730,15 @@
                     a response indicates an error during the exchange
         """
 
         # Currently, this only finds other UDP connections given a connection
         # that supports SCP - this is done via the machine
         if len(self._scamp_connections) == 0:
             return list()
+
         # if the machine hasn't been created, create it
         if self._machine is None:
             self._update_machine()
 
         # Find all the new connections via the machine Ethernet-connected chips
         new_connections = list()
         for chip in self._machine.ethernet_connected_chips:
@@ -742,14 +766,19 @@
 
                 # check if it works
                 if self._try_sver_though_scamp_connection(
                         MultiConnectionProcessMostDirectConnectionSelector(
                             None, [new_connection]), _STANDARD_RETIRES_NO):
                     self._scp_sender_connections.append(new_connection)
                     self._all_connections.add(new_connection)
+                else:
+                    logger.warn(
+                        "Additional Ethernet connection on {} at chip {}, {}"
+                        " cannot be contacted"
+                        .format(chip.ip_address, chip.x, chip.y))
 
         # Update the connection queues after finding new connections
         return new_connections
 
     def _search_for_proxies(self, chip):
         """ Looks for an entry within the UDP scamp connections which is\
             linked to a given chip
@@ -784,18 +813,25 @@
         :raise spinnman.exceptions.SpinnmanInvalidPacketException: If a packet\
                     is received that is not in the valid format
         :raise spinnman.exceptions.SpinnmanInvalidParameterException: If a\
                     packet is received that has invalid parameters
         :raise spinnman.exceptions.SpinnmanUnexpectedResponseCodeException: If\
                     a response indicates an error during the exchange
         """
-        if self._machine is None:
-            self._update_machine()
-        return MachineDimensions(self._machine.max_chip_x + 1,
-                                 self._machine.max_chip_y + 1)
+        if self._width is None or self._height is None:
+            height_item = SystemVariableDefinition.y_size
+            self._height, self._width = struct.unpack_from(
+                "<BB",
+                str(self.read_memory(
+                    AbstractSCPRequest.DEFAULT_DEST_X_COORD,
+                    AbstractSCPRequest.DEFAULT_DEST_Y_COORD,
+                    (constants.SYSTEM_VARIABLE_BASE_ADDRESS +
+                        height_item.offset),
+                    2)))
+        return MachineDimensions(self._width, self._height)
 
     def get_machine_details(self):
         """ Get the details of the machine made up of chips on a board and how\
             they are connected to each other.
 
         :return: A machine description
         :rtype: :py:class:`spinn_machine.machine.Machine`
@@ -830,15 +866,18 @@
             return False
         else:
             for connection in self._scamp_connections:
                 if connection.is_connected():
                     return True
             return False
 
-    def get_scamp_version(self, chip_x=0, chip_y=0, connection_selector=None):
+    def get_scamp_version(
+            self, chip_x=AbstractSCPRequest.DEFAULT_DEST_X_COORD,
+            chip_y=AbstractSCPRequest.DEFAULT_DEST_Y_COORD,
+            connection_selector=None):
         """ Get the version of scamp which is running on the board
 
         :param connection_selector: the connection to send the scamp
             version or none (if none then a random scamp connection is used)
         :type connection_selector: a instance of a
             :py:class:'spinnman.processes.abstract_multi_connection_process_connection_selector.AbstractMultiConnectionProcessConnectionSelector'
         :param chip_x: the chip's x coordinate to query for scamp version
@@ -856,58 +895,53 @@
         """
         if connection_selector is None:
             connection_selector = self._scamp_connection_selector
         process = GetVersionProcess(connection_selector)
         return process.get_version(x=chip_x, y=chip_y, p=0)
 
     def boot_board(
-            self, number_of_boards=1, width=None, height=None):
+            self, number_of_boards=None, width=None, height=None):
         """ Attempt to boot the board.  No check is performed to see if the\
             board is already booted.
 
-        :param number_of_boards: the number of boards that this machine is \
-                made out of, 1 by default
+        :param number_of_boards: this parameter is deprecated
         :type number_of_boards: int
-        :param width: The width of the machine in chips, or None to compute
+        :param width: this parameter is deprecated
         :type width: int or None
-        :param height: The height of the machine in chips, or None to compute
+        :param height: this parameter is deprecated
         :type height: int or None
         :raise spinnman.exceptions.SpinnmanInvalidParameterException: If the\
                     board version is not known
         :raise spinnman.exceptions.SpinnmanIOException: If there is an error\
                     communicating with the board
         """
-        logger.debug("Attempting to boot version {} board".format(
-            self._version))
-        if width is None or height is None:
-            dims = utility_functions.get_ideal_size(number_of_boards,
-                                                    self._version)
-            width = dims.width
-            height = dims.height
-        boot_messages = SpinnakerBootMessages(
-            self._version, number_of_boards=number_of_boards,
-            width=width, height=height)
+        if (width is not None or height is not None or
+                number_of_boards is not None):
+            logger.warning(
+                "The width, height and number_of_boards are no longer"
+                " supported, and might be removed in a future version")
+        boot_messages = SpinnakerBootMessages(board_version=self._version)
         for boot_message in boot_messages.messages:
             self._boot_send_connection.send_boot_message(boot_message)
         time.sleep(2.0)
 
     def ensure_board_is_ready(
-            self, number_of_boards=1, width=None, height=None,
+            self, number_of_boards=None, width=None, height=None,
             n_retries=5, enable_reinjector=True):
         """ Ensure that the board is ready to interact with this version\
             of the transceiver.  Boots the board if not already booted and\
             verifies that the version of SCAMP running is compatible with\
             this transceiver.
 
-        :param number_of_boards: the number of boards that this machine is
-                    constructed out of, 1 by default
+        :param number_of_boards: this parameter is deprecated and will be\
+                    ignored
         :type number_of_boards: int
-        :param width: The width of the machine in chips, or None to compute
+        :param width: this parameter is deprecated and will be ignored
         :type width: int or None
-        :param height: The height of the machine in chips, or None to compute
+        :param height: this parameter is deprecated and will be ignored
         :type height: int or None
         :param n_retries: The number of times to retry booting
         :type n_retries: int
         :param enable_reinjector: a boolean that allows the reinjector to be\
                     added to the system
         :type enable_reinjector: bool
         :return: The version identifier
@@ -915,28 +949,27 @@
         :raise: spinnman.exceptions.SpinnmanIOException:
                     * If there is a problem booting the board
                     * If the version of software on the board is not\
                       compatible with this transceiver
         """
 
         # if the machine sizes not been given, calculate from assumption
-        if width is None or width is None:
-            dims = utility_functions.get_ideal_size(number_of_boards,
-                                                    self._version)
-            width = dims.width
-            height = dims.height
+        if (width is not None or height is not None or
+                number_of_boards is not None):
+            logger.warning(
+                "The width, height and number_of_boards are no longer"
+                " supported, and might be removed in a future version")
 
         # try to get a scamp version once
         logger.info("Working out if machine is booted")
         version_info = self._try_to_find_scamp_and_boot(
             INITIAL_FIND_SCAMP_RETRIES_COUNT, number_of_boards, width, height)
 
         # If we fail to get a SCAMP version this time, try other things
-        if (version_info is None and self._version >= 4 and
-                len(self._bmp_connections) > 0):
+        if version_info is None and len(self._bmp_connections) > 0:
 
             # start by powering up each BMP connection
             logger.info("Attempting to power on machine")
             self.power_on_machine()
 
             # Sleep a bit to let things get going
             time.sleep(2.0)
@@ -956,16 +989,14 @@
                 "The machine is currently booted with {}"
                 " {} which is incompatible with this transceiver, "
                 "required version is {} {}".format(
                     version_info.name, version_info.version_number,
                     _SCAMP_NAME, _SCAMP_VERSION))
 
         else:
-            if self._machine is None:
-                self._update_machine()
             logger.info("Machine communication successful")
 
         # Change the default SCP timeout on the machine, keeping the old one to
         # revert at close
         for scamp_connection in self._scamp_connections:
             process = SendSingleCommandProcess(self._scamp_connection_selector)
             process.execute(SCPIPTagTTORequest(
@@ -992,14 +1023,20 @@
                 the machine
         """
         version_info = None
         current_tries_to_go = tries_to_go
         while version_info is None and current_tries_to_go > 0:
             try:
                 version_info = self.get_scamp_version()
+                if (version_info.x ==
+                        AbstractSCPRequest.DEFAULT_DEST_X_COORD) and \
+                        (version_info.y ==
+                         AbstractSCPRequest.DEFAULT_DEST_Y_COORD):
+                    version_info = None
+                    time.sleep(0.1)
             except exceptions.SpinnmanGenericProcessException as e:
                 if isinstance(
                         e.exception, exceptions.SpinnmanTimeoutException):
                     logger.info("Attempting to boot machine")
                     self.boot_board(number_of_boards, width, height)
                     current_tries_to_go -= 1
                 elif isinstance(
@@ -1016,114 +1053,71 @@
                 raise exceptions.SpinnmanIOException(
                     "Failed to communicate with the machine")
 
         # The last thing we tried was booting, so try again to get the version
         if version_info is None:
             try:
                 version_info = self.get_scamp_version()
+                if (version_info.x ==
+                        AbstractSCPRequest.DEFAULT_DEST_X_COORD) and \
+                        (version_info.y ==
+                         AbstractSCPRequest.DEFAULT_DEST_Y_COORD):
+                    version_info = None
             except exceptions.SpinnmanException:
                 pass
-
-        # boot has been sent, and 0 0 is up and running, but there will need to
-        # be a delay whilst all the other chips complete boot.
         if version_info is not None:
-            checker = CheckMachineBootedProcess(
-                self._scamp_connections[0], self._ignore_chips,
-                self._ignore_cores, self._max_core_id, self._max_sdram_size)
-            self._machine, self._chip_info = checker.check_machine_is_booted()
-            if self._machine is None:
-                return None
-            spinnaker_links = utilities.locate_spinnaker_links(
-                self._version, self._machine)
-            for spinnaker_link in spinnaker_links:
-                self._machine.add_spinnaker_link(spinnaker_link)
-            logger.info(
-                "Detected a machine on ip address {} which has {}".format(
-                    self._boot_send_connection.remote_ip_address,
-                    self._machine.cores_and_link_output_string()))
-
-            # update scamp connection selector with machine dynamics
-            self._scamp_connection_selector.set_machine(self._machine)
-
+            logger.info("Found board with version {}".format(version_info))
         return version_info
 
-    def _check_if_machine_has_wrap_arounds(self):
-        """ Determine if the machine has wrap-arounds, by querying the links\
-            from 0, 0
-        :return: true if a wrap around toroid, false otherwise
-        :rtype: bool
-        """
-        try:
-            # Try the left link
-            self.read_neighbour_memory(
-                x=0, y=0, link=3,
-                base_address=constants.SYSTEM_VARIABLE_BASE_ADDRESS,
-                length=constants.SYSTEM_VARIABLE_BYTES)
-            return True
-        except (exceptions.SpinnmanUnexpectedResponseCodeException,
-                exceptions.SpinnmanTimeoutException):
-
-            # Do Nothing - check the bottom link for wrap around
-            pass
-
-        try:
-
-            # Try the bottom link
-            self.read_neighbour_memory(
-                x=0, y=0, link=4,
-                base_address=constants.SYSTEM_VARIABLE_BASE_ADDRESS,
-                length=constants.SYSTEM_VARIABLE_BYTES)
-            return True
-        except (exceptions.SpinnmanUnexpectedResponseCodeException,
-                exceptions.SpinnmanTimeoutException):
-
-            # Do Nothing
-            pass
-
-        return False
-
     def get_cpu_information(self, core_subsets=None):
         """ Get information about the processors on the board
 
         :param core_subsets: A set of chips and cores from which to get\
                     the information.  If not specified, the information from\
                     all of the cores on all of the chips on the board are\
                     obtained
-        :type core_subsets: :py:class:`spinnman.model.core_subsets.CoreSubsets`
+        :type core_subsets: :py:class:`spinn_machine.core_subsets.CoreSubsets`
         :return: An iterable of the cpu information for the selected cores, or\
                     all cores if core_subsets is not specified
         :rtype: iterable of :py:class:`spinnman.model.cpu_info.CPUInfo`
         :raise spinnman.exceptions.SpinnmanIOException: If there is an error\
                     communicating with the board
         :raise spinnman.exceptions.SpinnmanInvalidPacketException: If a packet\
                     is received that is not in the valid format
         :raise spinnman.exceptions.SpinnmanInvalidParameterException:
                     * If chip_and_cores contains invalid items
                     * If a packet is received that has invalid parameters
         :raise spinnman.exceptions.SpinnmanUnexpectedResponseCodeException: If\
                     a response indicates an error during the exchange
         """
-        # Ensure that the information about each chip is present
-        if self._machine is None:
-            self._update_machine()
 
         # Get all the cores if the subsets are not given
         if core_subsets is None:
+            if self._machine is None:
+                self._update_machine()
             core_subsets = CoreSubsets()
-            for chip_info in self._chip_info.itervalues():
-                x = chip_info.x
-                y = chip_info.y
-                for p in chip_info.virtual_core_ids:
-                    core_subsets.add_processor(x, y, p)
+            for chip in self._machine.chips:
+                for processor in chip.processors:
+                    core_subsets.add_processor(
+                        chip.x, chip.y, processor.processor_id)
 
         process = GetCPUInfoProcess(self._scamp_connection_selector)
-        return process.get_cpu_info(self._chip_info, core_subsets)
+        cpu_info = process.get_cpu_info(core_subsets)
+        return cpu_info
+
+    def _get_sv_data(self, x, y, data_item):
+        return struct.unpack_from(
+            data_item.data_type.struct_code,
+            str(self.read_memory(
+                x, y,
+                constants.SYSTEM_VARIABLE_BASE_ADDRESS + data_item.offset,
+                data_item.data_type.value)))[0]
 
     def get_user_0_register_address_from_core(self, x, y, p):
-        """Get the address of user 0 for a given processor on the board
+        """ Get the address of user 0 for a given processor on the board
 
         :param x: the x-coordinate of the chip containing the processor
         :param y: the y-coordinate of the chip containing the processor
         :param p: The id of the processor to get the user 0 address from
         :type x: int
         :type y: int
         :type p: int
@@ -1133,83 +1127,43 @@
                     is received that is not in the valid format
         :raise spinnman.exceptions.SpinnmanInvalidParameterException:
                     * If x, y, p is not a valid processor
                     * If a packet is received that has invalid parameters
         :raise spinnman.exceptions.SpinnmanUnexpectedResponseCodeException: If\
                     a response indicates an error during the exchange
         """
-        # Ensure that the information about each chip is present
-        if self._machine is None:
-            self._update_machine()
-
-        # check the chip exists in the info
-        if not (x, y) in self._chip_info:
-            raise exceptions.SpinnmanInvalidParameterException(
-                "x, y", "{}, {}".format(x, y),
-                "Not a valid chip on the current machine")
-
-        # collect the chip info for the associated chip
-        chip_info = self._chip_info[(x, y)]
-
-        # check that p is a valid processor for this chip
-        if p not in chip_info.virtual_core_ids:
-            raise exceptions.SpinnmanInvalidParameterException(
-                "p", str(p), "Not a valid core on chip {}, {}".format(x, y))
-
-        # locate the base address for this chip info
-        base_address = (chip_info.cpu_information_base_address +
-                        (constants.CPU_INFO_BYTES * p))
-        base_address += constants.CPU_USER_0_START_ADDRESS
-        return base_address
+        return (
+            utility_functions.get_vcpu_address(p) +
+            constants.CPU_USER_0_START_ADDRESS)
 
     def get_user_1_register_address_from_core(self, x, y, p):
-        """Get the address of user 1 for a given processor on the board
+        """ Get the address of user 1 for a given processor on the board
 
         :param x: the x-coordinate of the chip containing the processor
         :param y: the y-coordinate of the chip containing the processor
-        :param p: The id of the processor to get the user 0 address from
+        :param p: The id of the processor to get the user 1 address from
         :type x: int
         :type y: int
         :type p: int
-        :return: The address for user 0 register for this processor
+        :return: The address for user 1 register for this processor
         :rtype: int
         :raise spinnman.exceptions.SpinnmanInvalidPacketException: If a packet\
                     is received that is not in the valid format
         :raise spinnman.exceptions.SpinnmanInvalidParameterException:
                     * If x, y, p is not a valid processor
                     * If a packet is received that has invalid parameters
         :raise spinnman.exceptions.SpinnmanUnexpectedResponseCodeException: If\
                     a response indicates an error during the exchange
         """
-        # Ensure that the information about each chip is present
-        if self._machine is None:
-            self._update_machine()
-
-        # check the chip exists in the info
-        if not (x, y) in self._chip_info:
-            raise exceptions.SpinnmanInvalidParameterException(
-                "x, y", "{}, {}".format(x, y),
-                "Not a valid chip on the current machine")
-
-        # collect the chip info for the associated chip
-        chip_info = self._chip_info[(x, y)]
-
-        # check that p is a valid processor for this chip
-        if p not in chip_info.virtual_core_ids:
-            raise exceptions.SpinnmanInvalidParameterException(
-                "p", str(p), "Not a valid core on chip {}, {}".format(x, y))
-
-        # locate the base address for this chip info
-        base_address = (chip_info.cpu_information_base_address +
-                        (constants.CPU_INFO_BYTES * p))
-        base_address += constants.CPU_USER_1_START_ADDRESS
-        return base_address
+        return (
+            utility_functions.get_vcpu_address(p) +
+            constants.CPU_USER_1_START_ADDRESS)
 
     def get_user_2_register_address_from_core(self, x, y, p):
-        """Get the address of user 2 for a given processor on the board
+        """ Get the address of user 2 for a given processor on the board
 
         :param x: the x-coordinate of the chip containing the processor
         :param y: the y-coordinate of the chip containing the processor
         :param p: The id of the processor to get the user 0 address from
         :type x: int
         :type y: int
         :type p: int
@@ -1219,37 +1173,17 @@
                     is received that is not in the valid format
         :raise spinnman.exceptions.SpinnmanInvalidParameterException:
                     * If x, y, p is not a valid processor
                     * If a packet is received that has invalid parameters
         :raise spinnman.exceptions.SpinnmanUnexpectedResponseCodeException: If\
                     a response indicates an error during the exchange
         """
-        # Ensure that the information about each chip is present
-        if self._machine is None:
-            self._update_machine()
-
-        # check the chip exists in the info
-        if not (x, y) in self._chip_info:
-            raise exceptions.SpinnmanInvalidParameterException(
-                "x, y", "{}, {}".format(x, y),
-                "Not a valid chip on the current machine")
-
-        # collect the chip info for the associated chip
-        chip_info = self._chip_info[(x, y)]
-
-        # check that p is a valid processor for this chip
-        if p not in chip_info.virtual_core_ids:
-            raise exceptions.SpinnmanInvalidParameterException(
-                "p", str(p), "Not a valid core on chip {}, {}".format(x, y))
-
-        # locate the base address for this chip info
-        base_address = (chip_info.cpu_information_base_address +
-                        (constants.CPU_INFO_BYTES * p))
-        base_address += constants.CPU_USER_2_START_ADDRESS
-        return base_address
+        return (
+            utility_functions.get_vcpu_address(p) +
+            constants.CPU_USER_2_START_ADDRESS)
 
     def get_cpu_information_from_core(self, x, y, p):
         """ Get information about a specific processor on the board
 
         :param x: The x-coordinate of the chip containing the processor
         :type x: int
         :param y: The y-coordinate of the chip containing the processor
@@ -1276,34 +1210,39 @@
     def get_iobuf(self, core_subsets=None):
         """ Get the contents of the IOBUF buffer for a number of processors
 
         :param core_subsets: A set of chips and cores from which to get\
                     the buffers.  If not specified, the buffers from\
                     all of the cores on all of the chips on the board are\
                     obtained
-        :type core_subsets: :py:class:`spinnman.model.core_subsets.CoreSubsets`
+        :type core_subsets: :py:class:`spinn_machine.core_subsets.CoreSubsets`
         :return: An iterable of the buffers, which may not be in the order\
                     of core_subsets
         :rtype: iterable of :py:class:`spinnman.model.io_buffer.IOBuffer`
         :raise spinnman.exceptions.SpinnmanIOException: If there is an error\
                     communicating with the board
         :raise spinnman.exceptions.SpinnmanInvalidPacketException: If a packet\
                     is received that is not in the valid format
         :raise spinnman.exceptions.SpinnmanInvalidParameterException:
                     * If chip_and_cores contains invalid items
                     * If a packet is received that has invalid parameters
         :raise spinnman.exceptions.SpinnmanUnexpectedResponseCodeException: If\
                     a response indicates an error during the exchange
         """
-        # Ensure that the information about each chip is present
-        if self._machine is None:
-            self._update_machine()
 
+        # making the assumption that all chips have the same iobuf size.
+        if self._iobuf_size is None:
+            self._iobuf_size = self._get_sv_data(
+                AbstractSCPRequest.DEFAULT_DEST_X_COORD,
+                AbstractSCPRequest.DEFAULT_DEST_Y_COORD,
+                SystemVariableDefinition.iobuf_size)
+
+        # read iobuf from machine
         process = ReadIOBufProcess(self._scamp_connection_selector)
-        return process.read_iobuf(self._chip_info, core_subsets)
+        return process.read_iobuf(self._iobuf_size, core_subsets)
 
     def get_iobuf_from_core(self, x, y, p):
         """ Get the contents of IOBUF for a given core
 
         :param x: The x-coordinate of the chip containing the processor
         :type x: int
         :param y: The y-coordinate of the chip containing the processor
@@ -1416,15 +1355,15 @@
 
     def execute_flood(self, core_subsets, executable, app_id, n_bytes=None):
         """ Start an executable running on multiple places on the board.  This\
             will be optimised based on the selected cores, but it may still\
             require a number of communications with the board to execute.
 
         :param core_subsets: Which cores on which chips to start the executable
-        :type core_subsets: :py:class:`spinnman.model.core_subsets.CoreSubsets`
+        :type core_subsets: :py:class:`spinn_machine.core_subsets.CoreSubsets`
         :param executable: The data that is to be executed.  Should be one of\
                     the following:
                     * An instance of AbstractDataReader
                     * A bytearray
         :type executable:\
                     :py:class:`spinnman.data.abstract_data_reader.AbstractDataReader`\
                     or bytearray
@@ -2295,18 +2234,16 @@
         :raise spinnman.exceptions.SpinnmanInvalidPacketException: If a packet\
                     is received that is not in the valid format
         :raise spinnman.exceptions.SpinnmanInvalidParameterException: If a\
                     packet is received that has invalid parameters
         :raise spinnman.exceptions.SpinnmanUnexpectedResponseCodeException: If\
                     a response indicates an error during the exchange
         """
-        if self._machine is None:
-            self._update_machine()
-        chip_info = self._chip_info[(x, y)]
-        base_address = chip_info.router_table_copy_address()
+        base_address = self._get_sv_data(
+            x, y, SystemVariableDefinition.router_table_copy_address)
         process = GetMultiCastRoutesProcess(
             self._scamp_connection_selector, app_id)
         return process.get_routes(x, y, base_address)
 
     def clear_multicast_routes(self, x, y):
         """ Remove all the multicast routes on a chip
 
@@ -2506,14 +2443,15 @@
         :rtype: None
         :raise None: No known exceptions are raised
         """
 
         if self._reinjection_running:
             process = ExitDPRIProcess(self._scamp_connection_selector)
             process.exit(self._reinjector_cores)
+            self.stop_application(_REINJECTOR_APP_ID)
             self._reinjection_running = False
 
         if power_off_machine and len(self._bmp_connections) > 0:
             self.power_off_machine()
 
         for receiving_connections in \
                 self._udp_receive_connections_by_port.values():
@@ -2666,17 +2604,22 @@
             # Find a free core on each chip to use
             for chip in self._machine.chips:
                 try:
                     first_processor = None
                     for processor in chip.processors:
                         if not processor.is_monitor:
                             first_processor = processor
-                    first_processor.is_monitor = True
-                    self._reinjector_cores.add_processor(
-                        chip.x, chip.y, first_processor.processor_id)
+                    if first_processor is not None:
+                        first_processor.is_monitor = True
+                        self._reinjector_cores.add_processor(
+                            chip.x, chip.y, first_processor.processor_id)
+                    else:
+                        logger.warn(
+                            "No processor on {}, {} was free to use for"
+                            " reinjection".format(chip.x, chip.y))
                 except StopIteration:
                     pass
 
             # Load the reinjector on each free core
             reinjector_binary = os.path.join(
                 os.path.dirname(model_binaries.__file__), "reinjector.aplx")
             reinjector_size = os.stat(reinjector_binary).st_size
```

## Comparing `SpiNNMan-2016.001/spinnman/__init__.py` & `SpiNNMan-3.0.0/spinnman/__init__.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/connection_listener.py` & `SpiNNMan-3.0.0/spinnman/connections/connection_listener.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/scp_request_pipeline.py` & `SpiNNMan-3.0.0/spinnman/connections/scp_request_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,16 @@
         for which a reply has not been received can also timeout.
     """
 
     def __init__(self, connection, n_channels=1,
                  intermediate_channel_waits=0,
                  retry_codes=set([SCPResult.RC_TIMEOUT,
                                   SCPResult.RC_P2P_TIMEOUT,
-                                  SCPResult.RC_LEN]),
+                                  SCPResult.RC_LEN,
+                                  SCPResult.RC_P2P_NOREPLY]),
                  n_retries=3, packet_timeout=0.5):
         """
         :param connection: The connection over which the communication is to\
                     take place
         :param n_channels: The number of requests to send before checking for\
                     responses.  If None, this will be determined automatically
         :param intermediate_channel_waits: The number of outstanding responses\
@@ -107,32 +108,32 @@
         self._request_data[_next_sequence] = request_data
         self._retries[_next_sequence] = self._n_retries
         self._callbacks[_next_sequence] = callback
         self._error_callbacks[_next_sequence] = error_callback
         self._send_time[_next_sequence] = time.time()
         _next_sequence = (_next_sequence + 1) % MAX_SEQUENCE
 
-        # Send the request, keeping track of how many are sent
-        # self._token_bucket.consume(284)
-        self._connection.send(request_data)
-        self._in_progress += 1
-
         # If the connection has not been measured
         if self._n_channels is None:
             if self._connection.is_ready_to_receive():
                 self._n_channels = self._in_progress + 8
                 if self._n_channels < 12:
                     self._n_channels = 12
                 self._intermediate_channel_waits = self._n_channels - 8
 
         # If all the channels are used, start to receive packets
         while (self._n_channels is not None and
                 self._in_progress >= self._n_channels):
             self._do_retrieve(self._intermediate_channel_waits, 0.1)
 
+        # Send the request, keeping track of how many are sent
+        # self._token_bucket.consume(284)
+        self._connection.send(request_data)
+        self._in_progress += 1
+
     def finish(self):
         """ Indicate the end of the packets to be sent.  This must be called\
             to ensure that all responses are received and handled.
         """
         while self._in_progress > 0:
             self._do_retrieve(0, self._packet_timeout)
```

## Comparing `SpiNNMan-2016.001/spinnman/connections/socket_address_with_chip.py` & `SpiNNMan-3.0.0/spinnman/connections/socket_address_with_chip.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/token_bucket.py` & `SpiNNMan-3.0.0/spinnman/connections/token_bucket.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_connection.py` & `SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_connection.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_eieio_receiver.py` & `SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_eieio_receiver.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_eieio_sender.py` & `SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_eieio_sender.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_listenable.py` & `SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_listenable.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_multicast_receiver.py` & `SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_multicast_receiver.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_multicast_sender.py` & `SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_multicast_sender.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_scp_receiver.py` & `SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_scp_receiver.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_scp_sender.py` & `SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_scp_sender.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_sdp_receiver.py` & `SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_sdp_receiver.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_sdp_sender.py` & `SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_sdp_sender.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_spinnaker_boot_receiver.py` & `SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_spinnaker_boot_receiver.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/abstract_classes/abstract_spinnaker_boot_sender.py` & `SpiNNMan-3.0.0/spinnman/connections/abstract_classes/abstract_spinnaker_boot_sender.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_bmp_connection.py` & `SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_bmp_connection.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_boot_connection.py` & `SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_boot_connection.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_connection.py` & `SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_connection.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_eieio_connection.py` & `SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_eieio_connection.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_ip_address_connection.py` & `SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_ip_address_connection.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_scamp_connection.py` & `SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_scamp_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 
 
 class UDPSCAMPConnection(UDPSDPConnection, AbstractSCPSender,
                          AbstractSCPReceiver):
     """ A UDP connection to SCAMP on the board
     """
 
-    def __init__(self, chip_x=0, chip_y=0, local_host=None, local_port=None,
-                 remote_host=None, remote_port=None):
+    def __init__(
+            self, chip_x=255, chip_y=255, local_host=None, local_port=None,
+            remote_host=None, remote_port=None):
         """
 
         :param chip_x: The x-coordinate of the chip on the board with this\
                 remote_host
         :type chip_x: int
         :param chip_y: The y-coordinate of the chip on the board with this\
                 remote_host
@@ -52,14 +53,18 @@
     def chip_x(self):
         return self._chip_x
 
     @property
     def chip_y(self):
         return self._chip_y
 
+    def update_chip_coordinates(self, x, y):
+        self._chip_x = x
+        self._chip_y = y
+
     def get_scp_data(self, scp_request):
         udp_utils.update_sdp_header_for_udp_send(scp_request.sdp_header,
                                                  self._chip_x, self._chip_y)
         return struct.pack("<2x") + scp_request.bytestring
 
     def receive_scp_response(self, timeout=1.0):
         data = self.receive(timeout)
```

## Comparing `SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_sdp_connection.py` & `SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_sdp_connection.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/connections/udp_packet_connections/udp_utils.py` & `SpiNNMan-3.0.0/spinnman/connections/udp_packet_connections/udp_utils.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/multicast_message.py` & `SpiNNMan-3.0.0/spinnman/messages/multicast_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/create_eieio_command.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/create_eieio_command.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/create_eieio_data.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/create_eieio_data.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/eieio_type.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/eieio_type.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/database_confirmation.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/database_confirmation.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/eieio_command_header.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/eieio_command_header.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/eieio_command_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/eieio_command_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/event_stop_request.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/event_stop_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/host_data_read.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/host_data_read.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/host_send_sequenced_data.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/host_send_sequenced_data.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/padding_request.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/padding_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/spinnaker_request_buffers.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/spinnaker_request_buffers.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/spinnaker_request_read_data.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/spinnaker_request_read_data.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/start_requests.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/start_requests.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/command_messages/stop_requests.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/command_messages/stop_requests.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/abstract_eieio_data_element.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/abstract_eieio_data_element.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_data_header.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_data_header.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_key_data_element.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_key_data_element.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_key_payload_data_element.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_key_payload_data_element.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_without_payload_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_without_payload_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_with_payload_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_with_payload_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_lower_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_lower_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_payload_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_payload_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_payload_prefix_lower_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_payload_prefix_lower_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_payload_prefix_upper_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_payload_prefix_upper_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_timed_payload_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_timed_payload_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_timed_payload_prefix_lower_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_timed_payload_prefix_lower_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_timed_payload_prefix_upper_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_timed_payload_prefix_upper_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_upper_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit/eieio_16bit_upper_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_lower_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_lower_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_payload_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_payload_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_payload_prefix_lower_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_payload_prefix_lower_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_payload_prefix_upper_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_payload_prefix_upper_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_timed_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_timed_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_timed_lower_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_timed_lower_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_timed_upper_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_timed_upper_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_upper_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_16bit_with_payload/eieio_16bit_with_payload_upper_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_lower_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_lower_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_payload_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_payload_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_payload_prefix_lower_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_payload_prefix_lower_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_payload_prefix_upper_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_payload_prefix_upper_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_timed_payload_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_timed_payload_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_timed_payload_prefix_lower_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_timed_payload_prefix_lower_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_timed_payload_prefix_upper_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_timed_payload_prefix_upper_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_upper_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit/eieio_32bit_upper_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_lower_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_lower_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_payload_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_payload_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_payload_prefix_lower_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_payload_prefix_lower_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_payload_prefix_upper_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_payload_prefix_upper_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_timed_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_timed_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_timed_lower_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_timed_lower_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_timed_upper_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_timed_upper_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_upper_key_prefix_data_message.py` & `SpiNNMan-3.0.0/spinnman/messages/eieio/data_messages/eieio_32bit_with_payload/eieio_32bit_with_payload_upper_key_prefix_data_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/scp_alloc_free_type.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/scp_alloc_free_type.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/scp_command.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/scp_command.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,20 +21,21 @@
     CMD_AS = 24
     CMD_LED = (25, "Control the LEDs")
     CMD_IPTAG = (26, "Set an IPTAG")
     CMD_SROM = 27
     CMD_ALLOC = (28, "Allocate or Free SDRAM or Routing entries")
     CMD_RTR = (29, "Initialise the router")
     CMD_DPRI = (30, "Dropped Packet Reinjection setup")
+    CMD_INFO = (31, "Get Chip Summary Information")
     CMD_BMP_INFO = (48, "Get BMP info structures")
     CMD_FLASH_COPY = 49
     CMD_FLASH_ERASE = 50
     CMD_FLASH_WRITE = 51
     CMD_RESET = 55
-    CMD_BMP_POWER = (57, "Turns on or off the machine via bmp")
+    CMD_BMP_POWER = (57, "Turns on or off the machine via BMP")
     CMD_TUBE = 64
 
     def __new__(cls, value, doc=""):
         obj = object.__new__(cls)
         obj._value_ = value
         return obj
```

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/scp_dpri_command.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/scp_dpri_command.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/scp_request_header.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/scp_request_header.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/scp_response_header.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/scp_response_header.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/scp_result.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/scp_result.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/scp_signal.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/scp_signal.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from enum import Enum
 
 
 class SignalType(Enum):
     """ The type of signal, determined by how it is transmitted
     """
-    MULTICAST = 0,
-    POINT_TO_POINT = 1,
+    MULTICAST = 0
+    POINT_TO_POINT = 1
     NEAREST_NEIGHBOUR = 2
 
 
 class SCPSignal(Enum):
     """ SCP Signals
     """
     INITIALISE = (0, SignalType.NEAREST_NEIGHBOUR)
     POWER_DOWN = (1, SignalType.NEAREST_NEIGHBOUR)
     STOP = (2, SignalType.NEAREST_NEIGHBOUR)
     START = (3, SignalType.NEAREST_NEIGHBOUR)
-    SYNC0 = (4, SignalType.NEAREST_NEIGHBOUR)
-    SYNC1 = (5, SignalType.NEAREST_NEIGHBOUR)
+    SYNC0 = (4, SignalType.MULTICAST)
+    SYNC1 = (5, SignalType.MULTICAST)
     PAUSE = (6, SignalType.MULTICAST)
     CONTINUE = (7, SignalType.MULTICAST)
-    EXIT = (8, SignalType.NEAREST_NEIGHBOUR)
+    EXIT = (8, SignalType.MULTICAST)
     TIMER = (9, SignalType.MULTICAST)
     USER_0 = (10, SignalType.MULTICAST)
     USER_1 = (11, SignalType.MULTICAST)
     USER_2 = (12, SignalType.MULTICAST)
     USER_3 = (13, SignalType.MULTICAST)
 
     def __new__(cls, value, signal_type, doc=""):
```

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/abstract_messages/abstract_scp_bmp_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/abstract_messages/abstract_scp_bmp_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/abstract_messages/abstract_scp_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/abstract_messages/abstract_scp_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 
 @add_metaclass(ABCMeta)
 class AbstractSCPRequest(object):
     """ Represents an Abstract SCP Request
     """
 
+    DEFAULT_DEST_X_COORD = 255
+    DEFAULT_DEST_Y_COORD = 255
+
     def __init__(self, sdp_header, scp_request_header, argument_1=None,
                  argument_2=None, argument_3=None, data=None):
         """
 
         :param sdp_header: The SDP header of the request
         :type sdp_header:\
                     :py:class:`spinnman.messages.sdp.sdp_header.SDPHeader`
```

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/abstract_messages/abstract_scp_response.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/abstract_messages/abstract_scp_response.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_application_run_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_application_run_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_app_stop_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_app_stop_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,16 +27,17 @@
         :type app_id: int
         :param signal: The signal to send
         :type signal: :py:class:`spinnman.messages.scp.scp_signal.SCPSignal`
         """
         super(SCPAppStopRequest, self).__init__(
             SDPHeader(
                 flags=SDPFlag.REPLY_EXPECTED, destination_port=0,
-                destination_cpu=0, destination_chip_x=0,
-                destination_chip_y=0),
+                destination_cpu=0,
+                destination_chip_x=self.DEFAULT_DEST_X_COORD,
+                destination_chip_y=self.DEFAULT_DEST_Y_COORD),
             SCPRequestHeader(command=SCPCommand.CMD_NNP),
             argument_1=(0x3f << 16),
             argument_2=(5 << 28) | _get_data(app_id, SCPSignal.STOP),
             argument_3=(1 << 31) + (0x3f << 8))
 
     def get_scp_response(self):
         return SCPCheckOKResponse("Send Stop", "CMD_NNP")
```

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_bmp_set_led_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_bmp_set_led_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_bmp_version_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_bmp_version_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_check_ok_response.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_check_ok_response.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_count_state_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_count_state_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,16 +32,17 @@
         :type app_id: int
         :param state: The state to count
         :type state: :py:class:`spinnman.model.cpu_state.CPUState`
         """
         super(SCPCountStateRequest, self).__init__(
             SDPHeader(
                 flags=SDPFlag.REPLY_EXPECTED, destination_port=0,
-                destination_cpu=0, destination_chip_x=0,
-                destination_chip_y=0),
+                destination_cpu=0,
+                destination_chip_x=self.DEFAULT_DEST_X_COORD,
+                destination_chip_y=self.DEFAULT_DEST_Y_COORD),
             SCPRequestHeader(command=SCPCommand.CMD_SIG),
             argument_1=_COUNT_SIGNAL_TYPE,
             argument_2=_get_data(app_id, state),
             argument_3=_ALL_CORE_MASK)
 
     def get_scp_response(self):
         return SCPCountStateResponse()
```

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_count_state_response.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_count_state_response.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_dpri_exit_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_dpri_exit_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_dpri_get_status_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_dpri_get_status_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_dpri_get_status_response.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_dpri_get_status_response.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_dpri_reset_counters_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_dpri_reset_counters_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_dpri_set_reinjection_packet_types.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_dpri_set_reinjection_packet_types.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_dpri_set_router_emergency_timeout_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_dpri_set_router_emergency_timeout_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_dpri_set_router_timeout_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_dpri_set_router_timeout_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_flood_fill_data_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_flood_fill_data_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,17 +34,19 @@
         if length is None:
             self._size = len(data)
 
         argument_1 = _NNP_FORWARD_RETRY | nearest_neighbour_id
         argument_2 = (block_no << 16) | (((self._size / 4) - 1) << 8)
 
         super(SCPFloodFillDataRequest, self).__init__(
-            SDPHeader(flags=SDPFlag.REPLY_EXPECTED, destination_port=0,
-                      destination_cpu=0, destination_chip_x=0,
-                      destination_chip_y=0),
+            SDPHeader(
+                flags=SDPFlag.REPLY_EXPECTED, destination_port=0,
+                destination_cpu=0,
+                destination_chip_x=self.DEFAULT_DEST_X_COORD,
+                destination_chip_y=self.DEFAULT_DEST_Y_COORD),
             SCPRequestHeader(command=SCPCommand.CMD_FFD),
             argument_1=argument_1, argument_2=argument_2,
             argument_3=base_address, data=None)
 
     @property
     def bytestring(self):
         datastring = super(SCPFloodFillDataRequest, self).bytestring
```

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_flood_fill_end_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_flood_fill_end_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
                 processor_mask |= (1 << processor)
 
         key = (_NNP_FLOOD_FILL_END << 24) | nearest_neighbour_id
         data = (app_id << 24) | processor_mask
 
         super(SCPFloodFillEndRequest, self).__init__(
             SDPHeader(flags=SDPFlag.REPLY_EXPECTED, destination_port=0,
-                      destination_cpu=0, destination_chip_x=0,
-                      destination_chip_y=0),
+                      destination_cpu=0,
+                      destination_chip_x=self.DEFAULT_DEST_X_COORD,
+                      destination_chip_y=self.DEFAULT_DEST_Y_COORD),
             SCPRequestHeader(command=SCPCommand.CMD_NNP),
             argument_1=key, argument_2=data, argument_3=_NNP_FORWARD_RETRY)
 
     def get_scp_response(self):
         return SCPCheckOKResponse("Flood Fill", "CMD_NNP:NNP_FFS")
```

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_flood_fill_start_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_router_alloc_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,42 @@
-from spinnman.messages.scp.abstract_messages.abstract_scp_request \
+from spinnman.messages.scp.abstract_messages.abstract_scp_request\
     import AbstractSCPRequest
 from spinnman.messages.sdp.sdp_header import SDPHeader
 from spinnman.messages.sdp.sdp_flag import SDPFlag
 from spinnman.messages.scp.scp_request_header import SCPRequestHeader
 from spinnman.messages.scp.scp_command import SCPCommand
-from spinnman.messages.scp.impl.scp_check_ok_response import SCPCheckOKResponse
+from spinnman.messages.scp.impl.scp_router_alloc_response\
+    import SCPRouterAllocResponse
+from spinnman.messages.scp.scp_alloc_free_type import SCPAllocFreeType
 
-_NNP_FORWARD_RETRY = (1 << 31) | (0x3f << 8) | 0x18
-_NNP_FLOOD_FILL_START = 6
 
-
-class SCPFloodFillStartRequest(AbstractSCPRequest):
-    """ A request to start a flood fill of data
+class SCPRouterAllocRequest(AbstractSCPRequest):
+    """ An SCP Request to allocate space for routing entries
     """
 
-    def __init__(self, nearest_neighbour_id, n_blocks, x=None, y=None):
+    def __init__(self, x, y, app_id, n_entries):
         """
 
-        :param nearest_neighbour_id: The id of the packet, between 0 and 127
-        :type nearest_neighbour_id: int
-        :param n_blocks: The number of blocks of data that will be sent,\
-                    between 0 and 255
-        :type n_blocks: int
-        :param x: The x-coordindate of the chip to load the data on to.  If\
-                    not specified, the data will be loaded on to all chips
+        :param x: The x-coordinate of the chip to allocate on, between 0 and\
+                    255
         :type x: int
-        :param y: The y-coordinate of the chip to load the data on to.  If\
-                    not specified, the data will be loaded on to all chips
+        :param y: The y-coordinate of the chip to allocate on, between 0 and\
+                    255
         :type y: int
+        :param app_id: The id of the application, between 0 and 255
+        :type app_id: int
+        :param n_entries: The number of entries to allocate
+        :type n_entries: int
         """
-        key = ((_NNP_FLOOD_FILL_START << 24) | (nearest_neighbour_id << 16) |
-               (n_blocks << 8))
-        data = 0xFFFF
-        if x is not None and y is not None:
-            m = ((y & 3) * 4) + (x & 3)
-            data = (((x & 0xfc) << 24) + ((y & 0xfc) << 16) +
-                    (3 << 16) + (1 << m))
-
-        super(SCPFloodFillStartRequest, self).__init__(
-            SDPHeader(flags=SDPFlag.REPLY_EXPECTED, destination_port=0,
-                      destination_cpu=0, destination_chip_x=0,
-                      destination_chip_y=0),
-            SCPRequestHeader(command=SCPCommand.CMD_NNP),
-            argument_1=key, argument_2=data, argument_3=_NNP_FORWARD_RETRY)
+        super(SCPRouterAllocRequest, self).__init__(
+            SDPHeader(
+                flags=SDPFlag.REPLY_EXPECTED, destination_port=0,
+                destination_cpu=0, destination_chip_x=x,
+                destination_chip_y=y),
+            SCPRequestHeader(command=SCPCommand.CMD_ALLOC),
+            argument_1=(
+                (app_id << 8) |
+                SCPAllocFreeType.ALLOC_ROUTING.value),  # @UndefinedVariable
+            argument_2=n_entries)
 
     def get_scp_response(self):
-        return SCPCheckOKResponse("Flood Fill", "CMD_NNP:NNP_FFS")
+        return SCPRouterAllocResponse()
```

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_iptag_clear_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_iptag_clear_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_iptag_get_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_iptag_get_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_iptag_get_response.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_iptag_get_response.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_iptag_info_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_iptag_info_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_iptag_info_response.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_iptag_info_response.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_iptag_set_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_iptag_set_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_iptag_tto_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_iptag_tto_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_led_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_led_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_power_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_power_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_adc_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_adc_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_adc_response.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_adc_response.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_fpga_register_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_fpga_register_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_fpga_register_response.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_fpga_register_response.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_link_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_link_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_link_response.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_link_response.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_memory_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_memory_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_read_memory_response.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_read_memory_response.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_reverse_iptag_set_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_reverse_iptag_set_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_router_alloc_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_sdram_de_alloc_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,59 @@
 from spinnman.messages.scp.abstract_messages.abstract_scp_request\
     import AbstractSCPRequest
+from spinnman.messages.scp.impl.scp_sdram_de_alloc_response import \
+    SCPSDRAMDeAllocResponse
 from spinnman.messages.sdp.sdp_header import SDPHeader
 from spinnman.messages.sdp.sdp_flag import SDPFlag
 from spinnman.messages.scp.scp_request_header import SCPRequestHeader
 from spinnman.messages.scp.scp_command import SCPCommand
-from spinnman.messages.scp.impl.scp_router_alloc_response\
-    import SCPRouterAllocResponse
 from spinnman.messages.scp.scp_alloc_free_type import SCPAllocFreeType
 
 
-class SCPRouterAllocRequest(AbstractSCPRequest):
-    """ An SCP Request to allocate space for routing entries
+class SCPSDRAMDeAllocRequest(AbstractSCPRequest):
+    """ An SCP Request to free space in the SDRAM
     """
 
-    def __init__(self, x, y, app_id, n_entries):
+    def __init__(self, x, y, app_id, base_address=None):
         """
 
         :param x: The x-coordinate of the chip to allocate on, between 0 and\
                     255
         :type x: int
         :param y: The y-coordinate of the chip to allocate on, between 0 and\
                     255
         :type y: int
         :param app_id: The id of the application, between 0 and 255
         :type app_id: int
-        :param n_entries: The number of entries to allocate
-        :type n_entries: int
+        :param base_address: The start address in SDRAM to which the block\
+                needs to be deallocated, or none if deallocating via app_id
+        :type base_address: int or None
         """
-        super(SCPRouterAllocRequest, self).__init__(
-            SDPHeader(
-                flags=SDPFlag.REPLY_EXPECTED, destination_port=0,
-                destination_cpu=0, destination_chip_x=x,
-                destination_chip_y=y),
-            SCPRequestHeader(command=SCPCommand.CMD_ALLOC),
-            argument_1=(
-                (app_id << 8) |
-                SCPAllocFreeType.ALLOC_ROUTING.value),  # @UndefinedVariable
-            argument_2=n_entries)
+
+        if base_address is not None:
+            AbstractSCPRequest.__init__(
+                self,
+                SDPHeader(
+                    flags=SDPFlag.REPLY_NOT_EXPECTED, destination_port=0,
+                    destination_cpu=0, destination_chip_x=x,
+                    destination_chip_y=y),
+                SCPRequestHeader(command=SCPCommand.CMD_ALLOC),
+                argument_1=(
+                    app_id << 8 |
+                    SCPAllocFreeType.
+                    FREE_SDRAM_BY_POINTER.value),  # @UndefinedVariable
+                argument_2=base_address)
+        else:
+            AbstractSCPRequest.__init__(
+                self,
+                SDPHeader(
+                    flags=SDPFlag.REPLY_EXPECTED, destination_port=0,
+                    destination_cpu=0, destination_chip_x=x,
+                    destination_chip_y=y),
+                SCPRequestHeader(command=SCPCommand.CMD_ALLOC),
+                argument_1=(
+                    app_id << 8 |
+                    SCPAllocFreeType.
+                    FREE_ROUTING_BY_APP_ID.value))  # @UndefinedVariable
 
     def get_scp_response(self):
-        return SCPRouterAllocResponse()
+        return SCPSDRAMDeAllocResponse()
```

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_router_alloc_response.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_router_alloc_response.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_router_clear_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_router_clear_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_router_init_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_router_init_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_sdram_alloc_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_sdram_alloc_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_sdram_alloc_response.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_sdram_alloc_response.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_sdram_de_alloc_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_chip_info_request.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,45 @@
 from spinnman.messages.scp.abstract_messages.abstract_scp_request\
     import AbstractSCPRequest
-from spinnman.messages.scp.impl.scp_sdram_de_alloc_response import \
-    SCPSDRAMDeAllocResponse
-from spinnman.messages.sdp.sdp_header import SDPHeader
 from spinnman.messages.sdp.sdp_flag import SDPFlag
+from spinnman.messages.sdp.sdp_header import SDPHeader
 from spinnman.messages.scp.scp_request_header import SCPRequestHeader
 from spinnman.messages.scp.scp_command import SCPCommand
-from spinnman.messages.scp.scp_alloc_free_type import SCPAllocFreeType
+from spinnman.messages.scp.impl.scp_chip_info_response \
+    import SCPChipInfoResponse
 
 
-class SCPSDRAMDeAllocRequest(AbstractSCPRequest):
-    """ An SCP Request to free space in the SDRAM
+class SCPChipInfoRequest(AbstractSCPRequest):
+    """ An SCP request to read the chip information from a core
     """
 
-    def __init__(self, x, y, app_id, base_address=None):
+    def __init__(self, x, y, with_size=False):
         """
 
-        :param x: The x-coordinate of the chip to allocate on, between 0 and\
-                    255
+        :param x: The x-coordinate of the chip to read from, between 0 and 255
         :type x: int
-        :param y: The y-coordinate of the chip to allocate on, between 0 and\
-                    255
+        :param y: The y-coordinate of the chip to read from, between 0 and 255
         :type y: int
-        :param app_id: The id of the application, between 0 and 255
-        :type app_id: int
-        :param base_address: The start address in SDRAM to which the block\
-                needs to be deallocated, or none if deallocating via app_id
-        :type base_address: int or None
+        :param with_size: True if the size should be included in the response,\
+                    False if not
+        :type with_size: bool
         """
-
-        if base_address is not None:
-            AbstractSCPRequest.__init__(
-                self,
-                SDPHeader(
-                    flags=SDPFlag.REPLY_NOT_EXPECTED, destination_port=0,
-                    destination_cpu=0, destination_chip_x=x,
-                    destination_chip_y=y),
-                SCPRequestHeader(command=SCPCommand.CMD_ALLOC),
-                argument_1=(
-                    app_id << 8 |
-                    SCPAllocFreeType.
-                    FREE_SDRAM_BY_POINTER.value),  # @UndefinedVariable
-                argument_2=base_address)
-        else:
-            AbstractSCPRequest.__init__(
-                self,
-                SDPHeader(
-                    flags=SDPFlag.REPLY_EXPECTED, destination_port=0,
-                    destination_cpu=0, destination_chip_x=x,
-                    destination_chip_y=y),
-                SCPRequestHeader(command=SCPCommand.CMD_ALLOC),
-                argument_1=(
-                    app_id << 8 |
-                    SCPAllocFreeType.
-                    FREE_ROUTING_BY_APP_ID.value))  # @UndefinedVariable
+        # Bits 0-4 + bit 6 = all information except size
+        argument_1 = 0x5F
+        if with_size:
+
+            # Bits 0-6 = all information including size
+            argument_1 = 0x7F
+
+        AbstractSCPRequest.__init__(
+            self, SDPHeader(
+                flags=SDPFlag.REPLY_EXPECTED, destination_port=0,
+                destination_cpu=0, destination_chip_x=x,
+                destination_chip_y=y),
+            SCPRequestHeader(command=SCPCommand.CMD_INFO),
+            argument_1=argument_1)
 
     def get_scp_response(self):
-        return SCPSDRAMDeAllocResponse()
+        """ See\
+            :py:meth:`spinnman.messages.scp.abstract_scp_request.AbstractSCPRequest.get_scp_response`
+        """
+        return SCPChipInfoResponse()
```

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_sdram_de_alloc_response.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_sdram_de_alloc_response.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_send_signal_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_send_signal_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,17 @@
         if app_id < 0 or app_id > 255:
             raise SpinnmanInvalidParameterException(
                 "app_id", str(app_id), "Must be between 0 and 255")
 
         super(SCPSendSignalRequest, self).__init__(
             SDPHeader(
                 flags=SDPFlag.REPLY_EXPECTED, destination_port=0,
-                destination_cpu=0, destination_chip_x=0,
-                destination_chip_y=0),
+                destination_cpu=0,
+                destination_chip_x=self.DEFAULT_DEST_X_COORD,
+                destination_chip_y=self.DEFAULT_DEST_Y_COORD),
             SCPRequestHeader(command=SCPCommand.CMD_SIG),
             argument_1=signal.signal_type.value,
             argument_2=_get_data(app_id, signal),
             argument_3=_ALL_CORE_MASK)
 
     def get_scp_response(self):
         return SCPCheckOKResponse("Send Signal", "CMD_SIG")
```

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_version_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_version_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_version_response.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_version_response.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_write_fpga_register_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_write_fpga_register_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_write_link_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_write_link_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/scp/impl/scp_write_memory_request.py` & `SpiNNMan-3.0.0/spinnman/messages/scp/impl/scp_write_memory_request.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/sdp/sdp_header.py` & `SpiNNMan-3.0.0/spinnman/messages/sdp/sdp_header.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/sdp/sdp_message.py` & `SpiNNMan-3.0.0/spinnman/messages/sdp/sdp_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/spinnaker_boot/spinnaker_boot_message.py` & `SpiNNMan-3.0.0/spinnman/messages/spinnaker_boot/spinnaker_boot_message.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/messages/spinnaker_boot/spinnaker_boot_messages.py` & `SpiNNMan-3.0.0/spinnman/messages/spinnaker_boot/spinnaker_boot_messages.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,87 +4,74 @@
 
 # spinnman imports
 from spinnman.messages.spinnaker_boot._system_variables import \
     _system_variable_boot_values as variable_boot_values
 from spinnman.messages.spinnaker_boot._system_variables.\
     _system_variable_boot_values import \
     SystemVariableDefinition
-import array
+from spinnman.messages.spinnaker_boot._system_variables\
+    ._system_variable_boot_values import SystemVariableBootValues
 from spinnman.messages.spinnaker_boot.spinnaker_boot_message \
     import SpinnakerBootMessage
 from spinnman.messages.spinnaker_boot.spinnaker_boot_op_code \
     import SpinnakerBootOpCode
 
 from spinnman.exceptions import SpinnmanInvalidParameterException
 from spinnman.exceptions import SpinnmanIOException
 
 # general imports
 import os
 import math
 import time
+import array
 
 _BOOT_MESSAGE_DATA_WORDS = 256
 _BOOT_MESSAGE_DATA_BYTES = _BOOT_MESSAGE_DATA_WORDS * 4
 _BOOT_IMAGE_MAX_BYTES = 32 * 1024
-_BOOT_DATA_FILE_NAME = "scamp-133.boot"
+_BOOT_DATA_FILE_NAME = "scamp-3.boot"
 _BOOT_STRUCT_REPLACE_OFFSET = 384 / 4
 _BOOT_STRUCT_REPLACE_LENGTH = 128 / 4
 _BOOT_DATA_OPERAND_1 = ((_BOOT_MESSAGE_DATA_BYTES / 4) - 1) << 8
 
 
 class SpinnakerBootMessages(object):
     """ Represents a set of boot messages to be sent to boot the board
     """
 
-    def __init__(
-            self, board_version, width, height, number_of_boards):
+    def __init__(self, board_version=None):
         """
         builds the boot messages needed to boot the spinnaker machine
 
         :param board_version: The version of the board to be booted
         :type board_version: int
-        :param width: The width of the machine in chips
-        :type width: int or None
-        :param height: The height of the machine in chips
-        :type height: int or None
-        :param number_of_boards: the number of boards that this spinnaker
-            machine is built up from
-        :type number_of_boards: int
         :raise spinnman.exceptions.SpinnmanInvalidParameterException: If the\
                     board version is not supported
         :raise spinnman.exceptions.SpinnmanIOException: If there is an error\
                     assembling the packets
         """
-        if board_version not in variable_boot_values.spinnaker_boot_values:
+        if (board_version is not None and
+                board_version not in
+                variable_boot_values.spinnaker_boot_values):
             raise SpinnmanInvalidParameterException(
                 "board_version", str(board_version), "Unknown board version")
 
         # Get the boot packet values
-        spinnaker_boot_value = \
-            variable_boot_values.spinnaker_boot_values[board_version]
+        if board_version is not None:
+            spinnaker_boot_value = variable_boot_values.spinnaker_boot_values[
+                board_version]
+        else:
+            spinnaker_boot_value = SystemVariableBootValues()
 
         current_time = int(time.time())
         spinnaker_boot_value.set_value(
             SystemVariableDefinition.unix_timestamp, current_time)
         spinnaker_boot_value.set_value(
             SystemVariableDefinition.boot_signature, current_time)
         spinnaker_boot_value.set_value(
             SystemVariableDefinition.is_root_chip, 1)
-        spinnaker_boot_value.set_value(
-            SystemVariableDefinition.x_size, int(width))
-        spinnaker_boot_value.set_value(
-            SystemVariableDefinition.y_size, int(height))
-
-        # add any updates for multi-board systems
-        for multi_board_n_boards, extra_variables in (
-                variable_boot_values
-                .spinnaker_multi_board_extra_configs.iteritems()):
-            if number_of_boards >= multi_board_n_boards:
-                for extra_variable, extra_value in extra_variables.iteritems():
-                    spinnaker_boot_value.set_value(extra_variable, extra_value)
 
         # Get the data as an array, to be used later
         self._spinnaker_boot_data = array.array(
             "I", spinnaker_boot_value.bytestring)
 
         # Find the data file and size
         this_dir, _ = os.path.split(__file__)
```

## Comparing `SpiNNMan-2016.001/spinnman/messages/spinnaker_boot/boot_data/scamp-133.boot` & `SpiNNMan-3.0.0/spinnman/messages/spinnaker_boot/boot_data/scamp-3.boot`

 * *Files 19% similar despite different names*

```diff
@@ -6,78 +6,78 @@
 00000050: 1219 103a e1ca e1c1 e1ca e1c1 203b f9d8  ...:........ ;..
 00000060: ece7 1d1c 1e1c 1f1c e8c1 e8c1 203a fbd8  ............ :..
 00000070: e4e7 0098 8847 e1e7 0000 0000 0000 0000  .....G..........
 00000080: 0200 0000 007f 0000 80ff ffff 8000 0000  ................
 00000090: 0200 0000 0070 0000 7001 0000 000e 0000  .....p..p.......
 000000a0: 0400 0000 187f 0000 0000 0000 0000 0000  ................
 000000b0: 0200 0000 007f 00f5 d000 0000 8000 0000  ................
-000000c0: 0200 0000 0000 0000 400f 0000 e04d 0000  ........@....M..
-000000d0: 0200 0000 0000 4000 105d 0000 2801 0000  ......@..]..(...
-000000e0: 0300 0000 2801 4000 e80a 0000 0000 0000  ....(.@.........
+000000c0: 0200 0000 0000 0000 400f 0000 8c58 0000  ........@....X..
+000000d0: 0200 0000 0000 4000 bc67 0000 3001 0000  ......@..g..0...
+000000e0: 0300 0000 3001 4000 1c0b 0000 0000 0000  ....0.@.........
 000000f0: 0400 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 41d8 a0e3 0400 8fe2 3300 90e8 0300 00fa  A.......3.......
 00000110: 8080 4000 0000 0000 d3f0 21e3 1eff 2fe1  ..@.......!.../.
 00000120: f2b5 0549 05a6 4027 3cce 3cc1 103f fbd1  ...I..@'<.<..?..
 00000130: 041c 3f39 0847 0000 c07f 0000 0fcc 0128  ..?9.G.........(
 00000140: 08d0 0228 04d0 0328 0bd0 0428 11d0 f2bd  ...(...(...(....
 00000150: 1219 103a e1ca e1c1 e1ca e1c1 203b f9d8  ...:........ ;..
 00000160: ece7 1d1c 1e1c 1f1c e8c1 e8c1 203a fbd8  ............ :..
 00000170: e4e7 0098 8847 e1e7 0000 0000 0000 0000  .....G..........
-00000180: 0000 0000 0000 0000 0000 0000 0004 3300  ..............3.
+00000180: 0000 0000 0000 0000 0000 0000 0404 3300  ..............3.
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001a0: 0000 0000 9600 8200 3f00 6432 520a 0202  ........?.d2R...
-000001b0: 0100 0000 0000 0000 0100 3201 0000 0000  ..........2.....
-000001c0: 0007 0a03 0100 0a01 0004 0000 0000 1000  ................
+000001a0: 0000 0000 c800 8200 3f00 6401 3200 0000  ........?.d.2...
+000001b0: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+000001c0: 0007 0a03 0000 0000 0004 0000 0000 1000  ................
 000001d0: 0040 0000 0000 8000 0080 0000 0000 0000  .@..............
-000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001e0: 0000 0000 003f 0000 0000 0000 0000 0000  .....?..........
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0200 0000 0000 0000 4000 0000 8c0a 0000  ........@.......
-00000210: 0300 0000 0000 4000 0401 0000 0000 0000  ......@.........
+00000200: 0200 0000 0000 0000 4000 0000 e40a 0000  ........@.......
+00000210: 0300 0000 0000 4000 1401 0000 0000 0000  ......@.........
 00000220: 0400 0000 0000 0000 0000 0000 0000 0000  ................
 00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000240: 18f0 9fe5 18f0 9fe5 18f0 9fe5 18f0 9fe5  ................
 00000250: 18f0 9fe5 faff ffeb f0ff 1fe5 18f0 9fe5  ................
 00000260: 7800 0000 d800 0000 e000 0000 e800 0000  x...............
 00000270: f000 0000 9d01 0000 f800 0000 0001 0000  ................
-00000280: 6000 4000 4000 0008 8c0a 0000 0401 4000  `.@.@.........@.
+00000280: 6000 4000 4000 0008 e40a 0000 1401 4000  `.@.@.........@.
 00000290: 0000 4100 adde adde 040f 1000 0000 0000  ..A.............
 000002a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000002b0: 0000 0000 0000 0000 6010 4fe2 bc03 c1e1  ........`.O.....
 000002c0: 4800 8fe2 0000 81e5 f400 9fe5 100f 01ee  H...............
 000002d0: d3f0 21e3 02d9 a0e3 6f00 00fa 54d0 1fe5  ..!.....o...T...
 000002e0: b226 5fe1 5810 1fe5 0200 4de0 9800 00eb  .&_.X.....M.....
-000002f0: 0d00 a0e1 2d01 00fa 00f0 21e1 3702 00fa  ....-.....!.7...
-00000300: fe01 00fa 3100 00fa f801 00fa 2a00 00eb  ....1.......*...
+000002f0: 0d00 a0e1 3501 00fa 00f0 21e1 4a02 00fa  ....5.....!.J...
+00000300: 1102 00fa 3100 00fa 0b02 00fa 2a00 00eb  ....1.......*...
 00000310: 0100 a0e3 1400 00ea 02b0 a0e3 0c00 00ea  ................
 00000320: 03b0 a0e3 0a00 00ea 04b0 a0e3 0800 00ea  ................
 00000330: 05b0 a0e3 0600 00ea 06b0 a0e3 0400 00ea  ................
 00000340: 07b0 a0e3 0200 00ea 08b0 a0e3 2f04 a0e3  ............/...
 00000350: 3000 90e5 0ea0 a0e1 0080 4fe1 c090 88e3  0.........O.....
 00000360: 2090 c9e3 09f0 2fe1 0200 00ea 00b0 a0e1   ...../.........
 00000370: 0080 0fe1 0ea0 a0e1 48c0 9fe5 00c0 9ce5  ........H.......
 00000380: 8090 a0e3 40e0 9fe5 9ce9 2ee0 0d90 a0e1  ....@...........
 00000390: ff07 8ee8 2cb0 cee5 0280 a0e3 2e80 cee5  ....,...........
 000003a0: 0b00 a0e1 d3f0 21e3 9900 00fa d3f0 21e3  ......!.......!.
 000003b0: 2f04 a0e3 0010 e0e3 1410 80e5 900f 07ee  /...............
-000003c0: fdff ffea 7e1f 0000 3000 4000 0070 00e5  ....~...0.@..p..
-000003d0: 0f20 00f0 c5f9 fff7 f2ef 0000 f2b5 0549  . .............I
+000003c0: fdff ffea 7e1f 0000 4000 4000 0070 00e5  ....~...@.@..p..
+000003d0: 0f20 00f0 d1f9 fff7 f2ef 0000 f2b5 0549  . .............I
 000003e0: 05a6 4027 3cce 3cc1 103f fbd1 041c 3f39  ..@'<.<..?....?9
 000003f0: 0847 0000 c07f 0000 0fcc 0128 08d0 0228  .G.........(...(
 00000400: 04d0 0328 0bd0 0428 11d0 f2bd 1219 103a  ...(...(.......:
 00000410: e1ca e1c1 e1ca e1c1 203b f9d8 ece7 1d1c  ........ ;......
 00000420: 1e1c 1f1c e8c1 e8c1 203a fbd8 e4e7 0098  ........ :......
 00000430: 8847 e1e7 0030 0fe1 01f0 21e1 00d0 a0e1  .G...0....!.....
 00000440: 03f0 2fe1 0201 40e0 1eff 2fe1 0000 0fe1  ../...@.../.....
 00000450: c010 80e3 01f0 21e1 1eff 2fe1 00f0 2fe1  ......!.../.../.
 00000460: 1eff 2fe1 e2c4 a0e3 00c1 8ce0 0000 0fe1  ../.............
 00000470: c010 80e3 01f0 21e1 0011 9ce5 0201 11e3  ......!.........
 00000480: fcff ff1a 1eff 2fe1 e2c4 a0e3 0111 8ce0  ....../.........
 00000490: 8011 91e5 00f0 21e1 1eff 2fe1 7047 0047  ......!.../.pG.G
 000004a0: 0f50 2de9 0400 4ee2 00c0 4fe1 1ff0 21e3  .P-...N...O...!.
-000004b0: 0050 2de9 fa00 00fa 0050 bde8 92f0 21e3  .P-......P....!.
+000004b0: 0050 2de9 0d01 00fa 0050 bde8 92f0 21e3  .P-......P....!.
 000004c0: 0cf0 6fe1 2f04 a0e3 3000 80e5 0f50 bde8  ..o./...0....P..
 000004d0: 04f0 5ee2 0120 d1e4 0000 52e3 0120 c0e4  ..^.. ....R.. ..
 000004e0: fbff ff1a 1eff 2fe1 900f 07ee 1eff 2fe1  ....../......./.
 000004f0: 0400 80e2 0410 81e2 b020 d1e1 0420 82e2  ......... ... ..
 00000500: 0300 12e3 0320 c213 0420 8212 1040 2de9  ..... ... ...@-.
 00000510: 2020 52e2 0500 003a 1850 b1e8 1850 a0e8    R....:.P...P..
 00000520: 1850 b1e8 1850 a0e8 2020 52e2 f9ff ff2a  .P...P..  R....*
@@ -86,133 +86,133 @@
 00000550: 1080 bde8 0130 a0e1 1020 52e2 0a00 a028  .....0... R....(
 00000560: 0a00 a028 fbff ff2a 822e b0e1 0a00 a028  ...(...*.......(
 00000570: 0200 a048 1eff 2fe1 01c0 5ee5 0c00 53e1  ...H../...^...S.
 00000580: 0330 de37 0c30 de27 83c0 8ee0 1cff 2fe1  .0.7.0.'....../.
 00000590: 70b5 0600 1821 00f0 43f8 0c4d 0400 0ed0  p....!..C..M....
 000005a0: 1822 3100 2000 00f0 47f8 0600 fff7 4eef  ."1. ...G.....N.
 000005b0: 2968 3160 2c60 fff7 52ef 0120 70bd 6869  )h1`,`..R.. p.hi
-000005c0: 0821 0843 6861 0020 70bd 0000 6c00 4000  .!.Cha. p...l.@.
+000005c0: 0821 0843 6861 0020 70bd 0000 7c00 4000  .!.Cha. p...|.@.
 000005d0: 70b5 0500 084c 03d0 0120 2076 0a20 02e0  p....L...  v. ..
-000005e0: 0020 2076 0720 00f0 bbf8 226b 002a 02d0  .  v. ...."k.*..
-000005f0: 616b 2800 9047 70bd 6c00 4000 0449 0222  ak(..Gp.l.@..I."
+000005e0: 0020 2076 0720 00f0 c7f8 226b 002a 02d0  .  v. ...."k.*..
+000005f0: 616b 2800 9047 70bd 7c00 4000 0449 0222  ak(..Gp.|.@..I."
 00000600: 0a76 1f23 ca6c 1b06 5a61 8863 7047 0000  .v.#.l..Za.cpG..
-00000610: 6c00 4000 0149 0820 c872 7047 207f 00e5  l.@..I. .rpG ...
-00000620: 4143 0448 0022 10b5 8069 1300 00f0 e2fa  AC.H."...i......
-00000630: 10bd 0000 3000 4000 0300 491e 02d0 8018  ....0.@...I.....
+00000610: 7c00 4000 0149 0820 c872 7047 207f 00e5  |.@..I. .rpG ...
+00000620: 4143 0448 0022 10b5 8069 1300 00f0 08fb  AC.H."...i......
+00000630: 10bd 0000 4000 4000 0300 491e 02d0 8018  ....@.@...I.....
 00000640: 1860 f9e7 0021 1960 7047 1430 10b5 07c8  .`...!.`pG.0....
 00000650: fff7 80ef 0020 10bd 70b5 0300 8069 ff22  ..... ..p....i."
 00000660: d969 0132 9042 01d8 0229 03d9 8420 1882  .i.2.B...)... ..
 00000670: 0020 70bd 5c69 1433 0029 06d1 02e0 625c  . p.\i.3.)....b\
 00000680: 5a54 491c 8142 fad3 70bd 0129 09d1 0021  ZTI..B..p..)...!
 00000690: 4508 03e0 4a00 a65a 491c 9e52 8d42 f9d8  E...J..ZI..R.B..
 000006a0: 70bd 0021 8508 03e0 8a00 a658 491c 9e50  p..!.......XI..P
-000006b0: 8d42 f9d8 70bd 0000 0a49 10b5 0988 0a04  .B..p....I......
-000006c0: 0949 4b68 0968 1b02 d218 5118 4161 0749  .IKh.h....Q.Aa.I
-000006d0: 8161 0749 0968 c161 2030 06a1 fff7 faee  .a.I.h.a 0......
-000006e0: 1b20 10bd 007f 00e5 3000 4000 0001 8500  . ......0.@.....
-000006f0: 7c0a 0000 5341 524b 2f53 7069 4e4e 616b  |...SARK/SpiNNak
-00000700: 6572 0000 30b5 ff23 8269 c169 0133 9a42  er..0..#.i.i.3.B
-00000710: 01d8 0229 02d9 8421 0182 1fe0 4369 2030  ...)...!....Ci 0
-00000720: 0029 06d1 02e0 445c 5c54 491c 9142 fad3  .)....D\\TI..B..
-00000730: 14e0 0129 09d1 0021 5408 03e0 4a00 855a  ...)...!T...J..Z
-00000740: 491c 9d52 8c42 f9d8 08e0 0021 9408 03e0  I..R.B.....!....
-00000750: 8a00 8558 491c 9d50 8c42 f9d8 0020 30bd  ...XI..P.B... 0.
-00000760: 0249 c969 2031 8873 7047 0000 3000 4000  .I.i 1.spG..0.@.
-00000770: 0300 2de9 0202 a0e3 1400 90e5 1000 9fe5  ..-.............
-00000780: 3810 90e5 0110 81e2 3810 80e5 0300 bde8  8.......8.......
-00000790: 04f0 5ee2 3000 4000 0200 0c32 0839 4260  ..^.0.@....2.9B`
-000007a0: c160 0260 0023 8160 0b60 0361 4b60 7047  .`.`.#.`.`.aK`pG
-000007b0: 70b5 4025 2988 0400 8900 401a 6a88 d221  p.@%).....@.j..!
-000007c0: fff7 38ee aa88 d121 fff7 34ee 0022 df21  ..8....!..4..".!
-000007d0: fff7 30ee e888 8108 8900 611a 2a4c 0020  ..0.......a.*L. 
-000007e0: 2161 c06c 6061 fff7 d7ff a061 2806 4069  !a.l`a.....a(.@i
-000007f0: 2649 000e 6060 4018 007d 2060 2348 ff26  &I..``@..} `#H.&
-00000800: 6038 8088 2086 2248 2536 a060 287e 3100  `8.. ."H%6.`(~1.
-00000810: fff7 06ff 2062 297e 3200 fff7 0dff 2168  .... b)~2.....!h
-00000820: 1229 1ed2 1b4a c801 8018 184a e061 403a  .)...J.....J.a@:
-00000830: 9369 5269 4b43 9900 8918 6163 7022 0021  .iRiKC....acp".!
-00000840: fff7 88ee e069 0522 0100 2031 8a73 2a7f  .....i.".. 1.s*.
-00000850: ca73 0e49 8039 c969 4164 0f49 4830 fff7  .s.I.9.iAd.IH0..
-00000860: 3aee 00f0 81f9 687e 0c4b 0122 1221 00f0  :.....h~.K.".!..
-00000870: 9bf9 0b4b 0122 0621 1020 00f0 95f9 a87e  ...K.".!. .....~
-00000880: fff7 86fe 1f20 70bd 3000 4000 807f 00e5  ..... p.0.@.....
-00000890: adde adde 0070 00e5 800a 0000 6002 0000  .....p......`...
-000008a0: 3005 0000 f8b5 0121 524f 7a68 9140 524a  0......!ROzh.@RJ
-000008b0: 8918 7122 5206 d160 fb69 1c00 2034 217e  ..q"R..`.i.. 4!~
-000008c0: 0029 18d0 1a6b 0229 00d1 1863 0025 2576  .)...k.)...c.%%v
-000008d0: 1f26 3606 0329 20d1 d31e fff7 4eee 0b11  .&6..) .....N...
-000008e0: 0c0c 0709 0d1c 1717 1717 0c00 0120 00e0  ............. ..
-000008f0: 0020 fff7 6dfe f8bd ff20 fff7 7ffe f8bd  . ..m.... ......
-00000900: 4020 417f 4908 4900 4177 f8bd 3b48 c262  @ A.I.I.Aw..;H.b
-00000910: 0120 4007 67e0 1020 65e0 0129 f5d1 0092  . @.g.. e..)....
-00000920: 00f0 80f8 0400 60d0 0099 2000 fff7 e0ed  ......`... .....
-00000930: 0098 00f0 edf8 b86a 401c b862 a77a 3806  .......j@..b.z8.
-00000940: 400f 31d1 a088 1828 01d2 8120 1be0 208a  @.1....(... .. .
-00000950: 8021 0028 2182 03d1 2000 fff7 adfe 14e0  .!.(!... .......
-00000960: 0228 03d1 2000 fff7 77fe 0ee0 0328 03d1  .(.. ...w....(..
-00000970: 2000 fff7 c7fe 08e0 0528 03d1 2000 fff7   ........(.. ...
-00000980: 64fe 02e0 8320 2082 2800 0c30 a080 a07a  d....  .(..0...z
-00000990: a189 e27a a272 e072 e089 a081 e181 0a21  ...z.r.r.......!
-000009a0: 2000 00f0 59f8 13e0 4020 c07e 0028 13d0   ...Y...@ .~.(..
-000009b0: 1348 8069 0028 0bd0 fff7 48ed 0500 7a09  .H.i.(....H...z.
-000009c0: 2100 0320 00f0 78f9 2800 fff7 48ed f8bd  !.. ..x.(...H...
-000009d0: 2000 00f0 17f8 f8bd 3069 c000 f8d5 0748   .......0i.....H
-000009e0: 8462 0120 0007 b061 f8bd 0098 00f0 90f8  .b. ...a........
-000009f0: f8bd 0000 3000 4000 0000 c05e 6c00 4000  ....0.@....^l.@.
-00000a00: 0000 4000 70b5 0500 054c fff7 20ed 216a  ..@.p....L.. .!j
-00000a10: 2960 2562 a18c 491e a184 fff7 20ed 70bd  )`%b..I..... .p.
-00000a20: 3000 4000 70b5 0b4c fff7 10ed 256a 2034  0.@.p..L....%j 4
-00000a30: 002d 0ad0 2968 2160 a188 491c 0904 090c  .-..)h!`..I.....
-00000a40: a180 e288 9142 00d9 e180 fff7 08ed 2800  .....B........(.
-00000a50: 70bd 0000 3000 4000 f8b5 0d00 0600 00f0  p...0.@.........
-00000a60: 69f8 0400 01d1 0020 f8bd 3100 2000 fff7  i...... ..1. ...
-00000a70: 40ed 1c4e 0127 f069 4463 2030 4776 3800  @..N.'.iDc 0Gv8.
-00000a80: fff7 f0ec 3268 1849 3b00 9340 c96a 164a  ....2h.I;..@.j.J
-00000a90: 0b43 0029 d362 08d1 1349 7122 2039 097a  .C.).b...Iq" 9.z
-00000aa0: 8f40 1249 7918 5206 9160 0121 fff7 ecec  .@.Iy.R..`.!....
-00000ab0: 0d49 b039 0a68 f069 2030 03e0 0b68 9b1a  .I.9.h.i 0...h..
-00000ac0: ab42 02d8 437e 002b f8d1 407e 0028 03d0  .B..C~.+..@~.(..
-00000ad0: 2000 00f0 1df8 c6e7 f06a 401c f062 0120   ........j@..b. 
-00000ae0: f8bd 0000 3000 4000 c07f 00e5 0000 c05e  ....0.@........^
-00000af0: 0248 0b21 c069 2030 8173 7047 3000 4000  .H.!.i 0.spG0.@.
-00000b00: 0248 0621 c069 2030 8173 7047 3000 4000  .H.!.i 0.spG0.@.
-00000b10: 10b5 0400 0020 fff7 a6ec 0549 0a68 2260  ..... .....I.h"`
-00000b20: 0c60 8a88 521e 8a80 0021 fff7 aeec 10bd  .`..R....!......
-00000b30: 687f 00e5 0020 10b5 fff7 94ec 0949 0c68  h.... .......I.h
-00000b40: 002c 0ad0 2268 0a60 8a88 521c 1204 120c  .,.."h.`..R.....
-00000b50: 8a80 cb88 9a42 00d9 ca80 0021 fff7 94ec  .....B.....!....
-00000b60: 2000 10bd 687f 00e5 0020 f0b5 c043 1f24   ...h.... ...C.$
-00000b70: 2406 6061 0022 e260 2263 074b 074d 084f  $.`a.".`"c.K.M.O
-00000b80: 1000 8100 ce18 3260 c919 0d60 401c 1028  ......2`...`@..(
-00000b90: f7d3 0448 6063 f0bd 0002 001f 0801 0000  ...H`c..........
-00000ba0: 0001 001f 9002 0000 70b5 0124 8c40 1f25  ........p..$.@.%
-00000bb0: 2d06 1028 03d1 0020 c363 ec60 08e0 064e  -..(... .c.`...N
-00000bc0: 8000 8619 3360 2023 1943 044b c018 0160  ....3` #.C.K...`
-00000bd0: 002a 00d0 2c61 70bd 0001 001f 0002 001f  .*..,ap.........
-00000be0: 10b5 4024 01e0 fff7 80ec 607f c007 fad1  ..@$......`.....
-00000bf0: 10bd 0000 ffb5 81b0 1600 1d00 0029 30d0  .............)0.
-00000c00: ff2e 2ed8 280a aa07 01d4 4020 007f 0002  ....(.....@ ....
-00000c10: 8719 002e 05d0 2748 ba00 c069 8058 0028  ......'H...i.X.(
-00000c20: 1fd1 c91c 8808 8000 0830 0290 e807 03d0  .........0......
-00000c30: 0620 fff7 18ec 8446 0198 0022 0468 08e0  . .....F...".h..
-00000c40: 0298 2168 2018 a042 05d9 8842 0cd9 2200  ..!h ..B...B..".
-00000c50: 6468 002c f4d1 e807 03d0 0621 6046 fff7  dh.,.......!`F..
-00000c60: 14ec 0020 05b0 f0bd 0300 0833 8b42 04d2  ... .......3.B..
-00000c70: 0160 2060 6168 4160 6060 002a 02d0 6068  .` `ahA```.*..`h
-00000c80: 5060 02e0 0198 6168 0160 e807 03d0 0621  P`....ah.`.....!
-00000c90: 6046 fff7 faeb 0120 0004 381a 002e 6060  `F..... ..8...``
-00000ca0: 05d0 0449 2000 c969 0830 ba00 8850 2000  ...I ..i.0...P .
-00000cb0: 0830 d7e7 c07f 00e5 7047 0000 b69d 2254  .0......pG...."T
-00000cc0: 7361 726b 0000 0000 adde adde 0000 0000  sark............
-00000cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000006b0: 8d42 f9d8 70bd 0000 10b5 0400 0d48 0088  .B..p........H..
+000006c0: 0104 0d48 4268 0068 1202 8918 0818 6061  ...HBh.h......`a
+000006d0: 0a48 a061 0a48 0ba1 0068 e061 2000 2030  .H.a.H...h.a . 0
+000006e0: fff7 f8ee 2000 2f30 0aa1 fff7 f4ee 2120  .... ./0......! 
+000006f0: 10bd 0000 007f 00e5 4000 4000 0001 ffff  ........@.@.....
+00000700: d40a 0000 5341 524b 2f53 7069 4e4e 616b  ....SARK/SpiNNak
+00000710: 6572 0000 332e 302e 3100 0000 30b5 ff23  er..3.0.1...0..#
+00000720: 8269 c169 0133 9a42 01d8 0229 02d9 8421  .i.i.3.B...)...!
+00000730: 0182 1fe0 4369 2030 0029 06d1 02e0 445c  ....Ci 0.)....D\
+00000740: 5c54 491c 9142 fad3 14e0 0129 09d1 0021  \TI..B.....)...!
+00000750: 5408 03e0 4a00 855a 491c 9d52 8c42 f9d8  T...J..ZI..R.B..
+00000760: 08e0 0021 9408 03e0 8a00 8558 491c 9d50  ...!.......XI..P
+00000770: 8c42 f9d8 0020 30bd 0249 c969 2031 8873  .B... 0..I.i 1.s
+00000780: 7047 0000 4000 4000 0300 2de9 0202 a0e3  pG..@.@...-.....
+00000790: 1400 90e5 1000 9fe5 3810 90e5 0110 81e2  ........8.......
+000007a0: 3810 80e5 0300 bde8 04f0 5ee2 4000 4000  8.........^.@.@.
+000007b0: 0200 1032 0839 8b1a 4260 083b 0161 c360  ...2.9..B`.;.a.`
+000007c0: 0260 0023 8160 0b60 4361 4b60 7047 0000  .`.#.`.`CaK`pG..
+000007d0: 70b5 4025 2988 0400 8900 401a 6a88 d221  p.@%).....@.j..!
+000007e0: fff7 28ee aa88 d121 fff7 24ee 0022 df21  ..(....!..$..".!
+000007f0: fff7 20ee e888 8108 8900 611a 344c 0020  .. .......a.4L. 
+00000800: 2161 c06c 6061 fff7 d3ff a061 2806 4069  !a.l`a.....a(.@i
+00000810: 3049 000e 6060 4018 007d 2060 2d48 ff26  0I..``@..} `-H.&
+00000820: 6038 8088 2086 2c48 2536 a060 287e 3100  `8.. .,H%6.`(~1.
+00000830: fff7 f6fe 2062 297e 3200 fff7 fdfe 7121  .... b)~2.....q!
+00000840: 4906 6068 496b c906 c90e 8842 2dd0 2168  I.`hIk.....B-.!h
+00000850: 224a 204b c801 8018 403b e061 9a69 4a43  "J K....@;.a.iJC
+00000860: 9100 5a69 8918 6163 7022 0021 fff7 72ee  ..Zi..acp".!..r.
+00000870: e069 0522 0100 2031 8a73 6268 4a73 2a7f  .i.".. 1.sbhJs*.
+00000880: ca73 1449 8039 c969 4164 1549 c165 1549  .s.I.9.iAd.I.e.I
+00000890: 4830 fff7 20ee 0f48 4030 c06b 0002 000e  H0.. ..H@0.k....
+000008a0: 0328 02d0 1420 fff7 62ed 00f0 83f9 687e  .(... ..b.....h~
+000008b0: 0d4b 0122 1221 00f0 9df9 0c4b 0122 0621  .K.".!.....K.".!
+000008c0: 1020 00f0 97f9 a87e fff7 62fe 1f20 70bd  . .....~..b.. p.
+000008d0: 4000 4000 807f 00e5 adde adde 0070 00e5  @.@..........p..
+000008e0: 0100 0300 d80a 0000 6002 0000 4805 0000  ........`...H...
+000008f0: f8b5 0121 524f 7a68 9140 524a 8918 7122  ...!ROzh.@RJ..q"
+00000900: 5206 d160 fb69 1c00 2034 217e 0029 18d0  R..`.i.. 4!~.)..
+00000910: 1a6b 0229 00d1 1863 0025 2576 1f26 3606  .k.)...c.%%v.&6.
+00000920: 0329 20d1 d31e fff7 28ee 0b11 0c0c 0709  .) .....(.......
+00000930: 0d1c 1717 1717 0c00 0120 00e0 0020 fff7  ......... ... ..
+00000940: 47fe f8bd ff20 fff7 59fe f8bd 4020 417f  G.... ..Y...@ A.
+00000950: 4908 4900 4177 f8bd 3b48 c262 0120 4007  I.I.Aw..;H.b. @.
+00000960: 67e0 1020 65e0 0129 f5d1 0092 00f0 80f8  g.. e..)........
+00000970: 0400 60d0 0099 2000 fff7 baed 0098 00f0  ..`... .........
+00000980: edf8 b86a 401c b862 a77a 3806 400f 31d1  ...j@..b.z8.@.1.
+00000990: a088 1828 01d2 8120 1be0 208a 8021 0028  ...(... .. ..!.(
+000009a0: 2182 03d1 2000 fff7 87fe 14e0 0228 03d1  !... ........(..
+000009b0: 2000 fff7 51fe 0ee0 0328 03d1 2000 fff7   ...Q....(.. ...
+000009c0: adfe 08e0 0528 03d1 2000 fff7 3efe 02e0  .....(.. ...>...
+000009d0: 8320 2082 2800 0c30 a080 a07a a189 e27a  .  .(..0...z...z
+000009e0: a272 e072 e089 a081 e181 0a21 2000 00f0  .r.r.......! ...
+000009f0: 59f8 13e0 4020 c07e 0028 13d0 1348 8069  Y...@ .~.(...H.i
+00000a00: 0028 0bd0 fff7 22ed 0500 7a09 2100 0320  .(...."...z.!.. 
+00000a10: 00f0 7ef9 2800 fff7 22ed f8bd 2000 00f0  ..~.(..."... ...
+00000a20: 17f8 f8bd 3069 c000 f8d5 0748 8462 0120  ....0i.....H.b. 
+00000a30: 0007 b061 f8bd 0098 00f0 90f8 f8bd 0000  ...a............
+00000a40: 4000 4000 0000 c05e 7c00 4000 0000 4000  @.@....^|.@...@.
+00000a50: 70b5 0500 054c fff7 faec 216a 2960 2562  p....L....!j)`%b
+00000a60: a18c 491e a184 fff7 faec 70bd 4000 4000  ..I.......p.@.@.
+00000a70: 70b5 0b4c fff7 eaec 256a 2034 002d 0ad0  p..L....%j 4.-..
+00000a80: 2968 2160 a188 491c 0904 090c a180 e288  )h!`..I.........
+00000a90: 9142 00d9 e180 fff7 e2ec 2800 70bd 0000  .B........(.p...
+00000aa0: 4000 4000 f8b5 0d00 0600 00f0 69f8 0400  @.@.........i...
+00000ab0: 01d1 0020 f8bd 3100 2000 fff7 1aed 1c4e  ... ..1. ......N
+00000ac0: 0127 f069 4463 2030 4776 3800 fff7 caec  .'.iDc 0Gv8.....
+00000ad0: 3268 1849 3b00 9340 c96a 164a 0b43 0029  2h.I;..@.j.J.C.)
+00000ae0: d362 08d1 1349 7122 2039 097a 8f40 1249  .b...Iq" 9.z.@.I
+00000af0: 7918 5206 9160 0121 fff7 c6ec 0d49 b039  y.R..`.!.....I.9
+00000b00: 0a68 f069 2030 03e0 0b68 9b1a ab42 02d8  .h.i 0...h...B..
+00000b10: 437e 002b f8d1 407e 0028 03d0 2000 00f0  C~.+..@~.(.. ...
+00000b20: 1df8 c6e7 f06a 401c f062 0120 f8bd 0000  .....j@..b. ....
+00000b30: 4000 4000 c07f 00e5 0000 c05e 0248 0b21  @.@........^.H.!
+00000b40: c069 2030 8173 7047 4000 4000 0248 0621  .i 0.spG@.@..H.!
+00000b50: c069 2030 8173 7047 4000 4000 10b5 0400  .i 0.spG@.@.....
+00000b60: 0020 fff7 80ec 0549 0a68 2260 0c60 8a88  . .....I.h"`.`..
+00000b70: 521e 8a80 0021 fff7 88ec 10bd 687f 00e5  R....!......h...
+00000b80: 0020 10b5 fff7 6eec 0949 0c68 002c 0ad0  . ....n..I.h.,..
+00000b90: 2268 0a60 8a88 521c 1204 120c 8a80 cb88  "h.`..R.........
+00000ba0: 9a42 00d9 ca80 0021 fff7 6eec 2000 10bd  .B.....!..n. ...
+00000bb0: 687f 00e5 0020 f0b5 c043 1f24 2406 6061  h.... ...C.$$.`a
+00000bc0: 0022 e260 2263 074b 074d 084f 1000 8100  .".`"c.K.M.O....
+00000bd0: ce18 3260 c919 0d60 401c 1028 f7d3 0448  ..2`...`@..(...H
+00000be0: 6063 f0bd 0002 001f 0801 0000 0001 001f  `c..............
+00000bf0: 9002 0000 70b5 0124 8c40 1f25 2d06 1028  ....p..$.@.%-..(
+00000c00: 03d1 0020 c363 ec60 08e0 064e 8000 8619  ... .c.`...N....
+00000c10: 3360 2023 1943 044b c018 0160 002a 00d0  3` #.C.K...`.*..
+00000c20: 2c61 70bd 0001 001f 0002 001f 10b5 4024  ,ap...........@$
+00000c30: 01e0 fff7 5aec 607f c007 fad1 10bd 0000  ....Z.`.........
+00000c40: ffb5 81b0 0600 1d00 0029 32d0 0398 ff28  .........)2....(
+00000c50: 2fd8 280a aa07 01d4 4020 007f 0202 0398  /.(.....@ ......
+00000c60: 1018 0090 0398 0028 06d0 2848 009a c069  .......(..(H...i
+00000c70: 9200 8058 0028 1cd1 c91c 8f08 bf00 0837  ...X.(.........7
+00000c80: e807 03d0 0620 fff7 eeeb 8446 3468 0022  ..... .....F4h."
+00000c90: 07e0 2168 e019 a042 05d9 8842 0cd9 2200  ..!h...B...B..".
+00000ca0: 6468 002c f5d1 e807 03d0 0621 6046 fff7  dh.,.......!`F..
+00000cb0: eceb 0020 05b0 f0bd 0300 0833 8b42 04d2  ... .......3.B..
+00000cc0: 0160 2060 6168 4160 6060 6068 002a 01d0  .` `ahA````h.*..
+00000cd0: 5060 00e0 3060 f068 c01b f060 e807 03d0  P`..0`.h...`....
+00000ce0: 0621 6046 fff7 d0eb 0098 0121 0904 401a  .!`F.......!..@.
+00000cf0: 6060 0398 0028 06d0 0449 2000 ca69 0099  ``...(...I ..i..
+00000d00: 0830 8900 5050 2000 0830 d3e7 c07f 00e5  .0..PP ..0......
+00000d10: 7047 0000 4b3f 8f57 7361 726b 0000 0000  pG..K?.Wsark....
+00000d20: adde adde 0000 0000 0000 0000 0000 0000  ................
 00000d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -253,1269 +253,1440 @@
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 18f0 9fe5 18f0 9fe5 18f0 9fe5 18f0 9fe5  ................
 00001010: 18f0 9fe5 faff ffeb f0ff 1fe5 18f0 9fe5  ................
 00001020: 7800 0000 d800 0000 e000 0000 e800 0000  x...............
-00001030: f000 0000 f536 0000 f800 0000 0001 0000  .....6..........
-00001040: 6000 4000 4000 0008 e04d 0000 100c 4000  `.@.@....M....@.
+00001030: f000 0000 6140 0000 f800 0000 0001 0000  ....a@..........
+00001040: 6000 4000 4000 0008 8c58 0000 4c0c 4000  `.@.@....X..L.@.
 00001050: 0040 4000 adde adde 040f 1000 0000 0000  .@@.............
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 6010 4fe2 bc03 c1e1  ........`.O.....
 00001080: 4800 8fe2 0000 81e5 f400 9fe5 100f 01ee  H...............
-00001090: d3f0 21e3 02d9 a0e3 d50c 00fb 54d0 1fe5  ..!.........T...
-000010a0: b226 5fe1 5810 1fe5 0200 4de0 210e 00eb  .&_.X.....M.!...
-000010b0: 0d00 a0e1 0f10 00fa 00f0 21e1 3e11 00fa  ..........!.>...
-000010c0: 0511 00fa d00c 00fa ff10 00fa 2a00 00eb  ............*...
+00001090: d3f0 21e3 02d9 a0e3 d40e 00fa 54d0 1fe5  ..!.........T...
+000010a0: b226 5fe1 5810 1fe5 0200 4de0 7c10 00eb  .&_.X.....M.|...
+000010b0: 0d00 a0e1 9e12 00fa 00f0 21e1 e113 00fa  ..........!.....
+000010c0: 9f13 00fa ce0e 00fb 9913 00fa 2a00 00eb  ............*...
 000010d0: 0100 a0e3 1400 00ea 02b0 a0e3 0c00 00ea  ................
 000010e0: 03b0 a0e3 0a00 00ea 04b0 a0e3 0800 00ea  ................
 000010f0: 05b0 a0e3 0600 00ea 06b0 a0e3 0400 00ea  ................
 00001100: 07b0 a0e3 0200 00ea 08b0 a0e3 2f04 a0e3  ............/...
 00001110: 3000 90e5 0ea0 a0e1 0080 4fe1 c090 88e3  0.........O.....
 00001120: 2090 c9e3 09f0 2fe1 0200 00ea 00b0 a0e1   ...../.........
 00001130: 0080 0fe1 0ea0 a0e1 48c0 9fe5 00c0 9ce5  ........H.......
 00001140: 8090 a0e3 40e0 9fe5 9ce9 2ee0 0d90 a0e1  ....@...........
 00001150: ff07 8ee8 2cb0 cee5 0280 a0e3 2e80 cee5  ....,...........
-00001160: 0b00 a0e1 d3f0 21e3 910e 00fa d3f0 21e3  ......!.......!.
+00001160: 0b00 a0e1 d3f0 21e3 ec10 00fa d3f0 21e3  ......!.......!.
 00001170: 2f04 a0e3 0010 e0e3 1410 80e5 900f 07ee  /...............
-00001180: fdff ffea 7e1f 0000 3c0b 4000 0070 00e5  ....~...<.@..p..
+00001180: fdff ffea 7e1f 0000 780b 4000 0070 00e5  ....~...x.@..p..
 00001190: 04e0 4ee2 0140 2de9 00e0 4fe1 0050 2de9  ..N..@-...O..P-.
-000011a0: 1ff0 21e3 0e40 2de9 ee0a 00fb 0e40 bde8  ..!..@-......@..
+000011a0: 1ff0 21e3 0e40 2de9 160c 00fb 0e40 bde8  ..!..@-......@..
 000011b0: 92f0 21e3 2fc4 a0e3 30c0 8ce5 0050 bde8  ..!./...0....P..
 000011c0: 0ef0 6fe1 0180 fde8 10b5 344c 0020 e061  ..o.......4L. .a
-000011d0: 0a20 03f0 d5fa 0120 e061 10bd f8b5 0500  . ..... .a......
+000011d0: 0a20 03f0 8bff 0120 e061 10bd f8b5 0500  . ..... .a......
 000011e0: 0e00 2e4f fc69 12e0 002d 02da 0420 0443  ...O.i...-... .C
-000011f0: 01e0 0420 8443 fc61 0120 03f0 c1fa 1020  ... .C.a. ..... 
-00001200: 2043 f861 0120 03f0 bbfa fc61 6d00 761e   C.a. .....am.v.
+000011f0: 01e0 0420 8443 fc61 0120 03f0 77ff 1020  ... .C.a. ..w.. 
+00001200: 2043 f861 0120 03f0 71ff fc61 6d00 761e   C.a. ..q..am.v.
 00001210: ead2 f8bd 70b5 214d ec69 8604 2048 0e43  ....p.!M.i.. H.C
 00001220: 0643 0820 2043 e861 2021 6817 fff7 d6ff  .C.  C.a !h.....
 00001230: 2021 3000 fff7 d2ff ec61 70bd f8b5 0500   !0......ap.....
 00001240: 164f fc69 0820 2043 f861 2021 7817 fff7  .O.i.  C.a !x...
 00001250: c5ff a804 f903 0843 0e21 fff7 bfff fc61  .......C.!.....a
 00001260: 0221 0020 fff7 baff fe69 1025 0024 2800  .!. .....i.%.$(.
-00001270: 3043 0090 0ee0 0120 03f0 82fa f869 6400  0C..... .....id.
+00001270: 3043 0090 0ee0 0120 03f0 38ff f869 6400  0C..... ..8..id.
 00001280: 8007 01d5 0120 0443 0098 f861 0120 03f0  ..... .C...a. ..
-00001290: 77fa fe61 6d1e eed2 2000 f8bd 00c0 00e4  w..am... .......
+00001290: 2dff fe61 6d1e eed2 2000 f8bd 00c0 00e4  -..am... .......
 000012a0: 0000 0250 feb5 0600 4469 4548 0068 0090  ...P....DiEH.h..
 000012b0: 00f0 4df8 2006 08d5 00f0 41f8 0320 0821  ..M. .....A.. .!
 000012c0: 4006 00f0 4ff8 00f0 42f8 00f0 38f8 a106  @...O...B...8...
 000012d0: b069 890e 00f0 46f8 270c 3500 2035 1436  .i....F.'.5. 5.6
 000012e0: 0197 0de0 e005 06d5 2878 6d1c 0006 0821  ........(xm....!
 000012f0: 00f0 38f8 03e0 00f0 46f8 3070 761c 7f1e  ..8.....F.0pv...
 00001300: 002f efd1 00f0 23f8 0526 3606 0ce0 00f0  ./....#..&6.....
 00001310: 16f8 0821 3000 00f0 25f8 00f0 34f8 0500  ...!0...%...4...
 00001320: 00f0 15f8 e807 01d0 6006 f0d4 2449 0098  ........`...$I..
 00001330: 0860 e005 01d5 0020 febd 0198 febd 2049  .`..... ...... I
-00001340: 2020 10b5 c860 0120 03f0 1afa 10bd 0120    ...`. ....... 
-00001350: 10b5 03f0 15fa 1a49 2020 8860 0120 03f0  .......I  .`. ..
-00001360: 0ffa 10bd f8b5 0400 0d00 154f 0826 002c  ...........O.&.,
+00001340: 2020 10b5 c860 0120 03f0 d0fe 10bd 0120    ...`. ....... 
+00001350: 10b5 03f0 cbfe 1a49 2020 8860 0120 03f0  .......I  .`. ..
+00001360: c5fe 10bd f8b5 0400 0d00 154f 0826 002c  ...........O.&.,
 00001370: 01da be60 00e0 fe60 00f0 15f8 6400 6d1e  ...`...`....d.m.
 00001380: f5d1 fe60 f8bd f8b5 0024 0825 0c4e 0127  ...`.....$.%.N.'
 00001390: b068 4007 00d5 3c43 00f0 05f8 6400 6d1e  .h@...<C....d.m.
-000013a0: f6d1 6008 f8bd 70b5 0120 03f0 e9f9 044d  ..`...p.. .....M
-000013b0: 1024 ac60 0120 03f0 e3f9 ec60 70bd 0000  .$.`. .....`p...
+000013a0: f6d1 6008 f8bd 70b5 0120 03f0 9ffe 044d  ..`...p.. .....M
+000013b0: 1024 ac60 0120 03f0 99fe ec60 70bd 0000  .$.`. .....`p...
 000013c0: 4000 00e2 d049 0022 10b5 0a60 8378 4279  @....I."...`.xBy
 000013d0: 1b06 1a43 c378 0479 1b04 2402 2343 1a43  ...C.x.y..$.#C.C
 000013e0: 4a61 0278 4078 1202 0243 8a61 c748 0860  Ja.x@x...C.a.H.`
 000013f0: 10bd 0288 0a80 4288 4a80 8088 8880 7047  ......B.J.....pG
 00001400: 0288 0a80 4088 4880 7047 0288 0b88 9a42  ....@.H.pG.....B
 00001410: 05d1 4088 4988 8842 01d1 0120 7047 0020  ..@.I..B... pG. 
 00001420: 7047 30b5 0d00 4521 1170 0021 1400 5170  pG0...E!.p.!..Qp
 00001430: 1a02 1b04 1b0e 1a43 6280 4022 a180 e280  .......Cb.@"....
 00001440: 2272 6572 6181 0288 2282 4088 2100 6082  "rera...".@.!.`.
 00001450: af48 0c31 fff7 d4ff 0022 1421 2000 00f0  .H.1.....".! ...
 00001460: 60e9 c043 0102 0004 000e 0143 6181 30bd  `..C.......Ca.0.
 00001470: 70b5 0600 0c00 1500 1800 3100 fff7 b9ff  p.........1.....
 00001480: a348 b11d 801f fff7 b4ff 2802 2904 090e  .H........(.)...
 00001490: 9d4d 0843 b081 6868 c007 fcd1 3920 2200  .M.C..hh....9 ".
-000014a0: 3100 8006 03f0 1eea 3c2c 00d2 3c24 ac60  1.......<,..<$.`
+000014a0: 3100 8006 03f0 d4ee 3c2c 00d2 3c24 ac60  1.......<,..<$.`
 000014b0: ec60 70bd ffb5 81b0 1500 1e00 924c 6168  .`p..........Lah
 000014c0: c907 fcd1 3927 0100 bf06 2a00 3800 03f0  ....9'....*.8...
-000014d0: 6ae8 0299 3200 e819 03f0 64e8 7019 3c28  j...2.....d.p.<(
+000014d0: 54ec 0299 3200 e819 03f0 4eec 7019 3c28  T...2.....N.p.<(
 000014e0: 00d2 3c20 a060 e060 05b0 f0bd f8b5 0600  ..< .`.`........
 000014f0: 1000 0f00 ff22 0699 0132 f281 0822 3282  ....."...2..."2.
 00001500: 0622 b274 0422 f274 0a02 0904 090e 0a43  .".t.".t.......C
 00001510: 3400 3100 0e34 2031 b282 fff7 6aff 1988  4.1..4 1....j...
 00001520: 2183 5988 7a48 6183 2100 0831 801f fff7  !.Y.zHa.!..1....
 00001530: 60ff 2100 7648 0e31 fff7 62ff 754a 3b00  `.!.vH.1..b.uJ;.
 00001540: 2a21 3000 fff7 94ff f8bd 7149 10b5 0839  *!0.......qI...9
 00001550: 8c68 0a00 1169 0268 0300 0c40 0a40 9442  .h...i.h...@.@.B
 00001560: 8cb0 01d0 6a4b 1b1d 1988 8180 5988 0122  ....jK......Y.."
 00001570: c180 0092 684a 01a8 1100 0839 fff7 b6ff  ....hJ.....9....
 00001580: 0cb0 10bd f7b5 8cb0 0100 04ae 0236 2a22  .............6*"
-00001590: 01a8 03f0 a8e9 5c48 0061 3000 5c49 1830  ......\H.a0.\I.0
+00001590: 01a8 03f0 5eee 5c48 0061 3000 5c49 1830  ....^.\H.a0.\I.0
 000015a0: fff7 33ff 0028 11d0 6b46 198b 0806 000c  ..3..(..kF......
 000015b0: 090a 0843 0128 0bd1 0222 3300 0e33 02a9  ...C.(..."3..3..
 000015c0: 0092 9a1f 0231 01a8 fff7 90ff 0fb0 f0bd  .....1..........
 000015d0: 0228 fbd1 0025 3000 0e30 504c 8446 16e0  .(...%0..0PL.F..
 000015e0: e789 b804 11d5 211d 6046 fff7 0eff 0028  ......!.`F.....(
 000015f0: 0bd0 3000 211d 0830 fff7 fbfe 0120 4003  ..0.!..0..... @.
 00001600: 8743 8000 0743 e781 e0e7 2034 6d1c 0e98  .C...C.... 4m...
 00001610: 8542 e5d3 dae7 f0b5 8a29 a3b0 3a4c 02d9  .B.......)..:L..
-00001620: 2461 23b0 f0bd 0a00 0100 6846 03f0 5ae9  $a#.......hF..Z.
+00001620: 2461 23b0 f0bd 0a00 0100 6846 03f0 10ee  $a#.......hF....
 00001630: 2461 03ae 07a8 3649 0236 0230 fff7 e5fe  $a....6I.6.0....
 00001640: 0028 eed0 6b46 987b 0007 850e 6846 4419  .(..kF.{....hFD.
 00001650: a07b 0e34 0828 e4d1 188a 3200 0106 090c  .{.4.(....2.....
 00001660: 000a 0143 4f1b 3b00 3000 1433 0121 0c30  ...CO.;.0..3.!.0
 00001670: fff7 d7fe 142d 06d9 08ac 0234 6119 3a00  .....-.....4a.:.
-00001680: 2000 03f0 dce8 0020 2070 6070 0200 6080   ......  p`p..`.
+00001680: 2000 03f0 92ed 0020 2070 6070 0200 6080   ......  p`p..`.
 00001690: 3900 2000 00f0 44e8 c043 0102 0004 000e  9. ...D..C......
 000016a0: 0143 6180 0122 3900 01ab 0233 d202 2231  .Ca.."9....3.."1
 000016b0: 6846 fff7 ddfe b4e7 30b5 0d00 1902 1b04  hF......0.......
 000016c0: 1b0e 1943 4184 1102 1204 120e 1143 2a04  ...CA........C*.
 000016d0: 8184 2902 120e 1143 c184 0400 0021 2234  ..)....C.....!"4
 000016e0: 0a00 e180 0821 1a30 00f0 1ae8 4219 1132  .....!.0....B..2
 000016f0: 2900 2000 00f0 14e8 c043 0102 0004 000e  ). ......C......
 00001700: 0143 e180 30bd 0000 00c0 00e4 5b04 0000  .C..0.......[...
-00001710: 5c07 4000 0608 0000 2c49 0000 0c09 4000  \.@.....,I....@.
+00001710: 8807 4000 0608 0000 d053 0000 3809 4000  ..@......S..8.@.
 00001720: 0100 11e3 0030 a0e1 0200 a0e1 0110 4112  .....0........A.
 00001730: 04e0 2de5 0120 d317 0204 8010 0020 a0e3  ..-.. ....... ..
 00001740: 0100 52e1 02c0 8330 01c0 dc35 02e0 d337  ..R....0...5...7
 00001750: 0220 8232 0ec4 8c30 0c00 8030 f7ff ff3a  . .2...0...0...:
 00001760: 0200 00ea 0018 a0e1 2118 a0e1 2008 81e0  ........!... ...
 00001770: 2018 b0e1 faff ff1a 04f0 9de4 7123 5b06   ...........q#[.
-00001780: 5a68 0029 01d0 8243 00e0 0243 a648 1018  Zh.)...C...C.H..
-00001790: 5860 7047 70b5 04f0 aff8 a34c 7125 0119  X`pGp......Lq%..
-000017a0: 6d06 a961 0121 fff7 e9ff 0520 02f0 e8ff  m..a.!..... ....
-000017b0: ac61 70bd f0b5 0d06 0123 9c49 2d0e 1206  .ap......#.I-...
-000017c0: 0e68 120e 10e0 0121 9940 0142 0bd0 984c  .h.....!.@.B...L
-000017d0: d901 0919 0c00 974f 2034 a573 ff69 4f64  .......O 4.s.iOd
-000017e0: 9549 e273 ca54 5b1c b342 ecd3 f0bd 0100  .I.s.T[..B......
+00001780: 5a68 0029 01d0 8243 00e0 0243 a748 1018  Zh.)...C...C.H..
+00001790: 5860 7047 70b5 04f0 01fe a44c 7125 0119  X`pGp......Lq%..
+000017a0: 6d06 a961 0121 fff7 e9ff 0520 03f0 9efc  m..a.!..... ....
+000017b0: ac61 70bd f0b5 0d06 0123 9d49 2d0e 1206  .ap......#.I-...
+000017c0: 0e68 120e 10e0 0121 9940 0142 0bd0 994c  .h.....!.@.B...L
+000017d0: d901 0919 0c00 984f 2034 a573 ff69 4f64  .......O 4.s.iOd
+000017e0: 9649 e273 ca54 5b1c b342 ecd3 f0bd 0100  .I.s.T[..B......
 000017f0: 0020 0123 00e0 401c 0029 03d0 1a00 8240  . .#..@..).....@
 00001800: 0a42 f8d0 7047 f3b5 81b0 8d03 ad0b 2bd0  .B..pG........+.
-00001810: 0802 870e 8748 0e0e c030 406a f100 4418  .....H...0@j..D.
+00001810: 0802 870e 8848 0e0e c030 406a f100 4418  .....H...0@j..D.
 00001820: 2078 0028 06d1 6070 a070 6060 2800 fff7   x.(..`p.p``(...
-00001830: deff e070 2800 03f0 2dfc 2178 4018 2070  ...p(...-.!x@. p
-00001840: 6068 2843 6060 7d48 8561 3200 0421 2800  `h(C``}H.a2..!(.
+00001830: deff e070 2800 04f0 2bf9 2178 4018 2070  ...p(...+.!x@. p
+00001840: 6068 2843 6060 7e48 8561 3200 0421 2800  `h(C``~H.a2..!(.
 00001850: fff7 b0ff e520 0199 0006 0161 3902 8919  ..... .....a9...
-00001860: 4161 2800 fff7 96ff febd 7048 70b5 0124  Aa(.......pHp..$
+00001860: 4161 2800 fff7 96ff febd 7148 70b5 0124  Aa(.......qHp..$
 00001870: 0068 ff22 8440 7f21 e520 a41e 0132 0902  .h.".@.!. ...2..
-00001880: 0006 03f0 30e8 6b4d 0f22 c035 0721 a868  ....0.kM.".5.!.h
-00001890: 1202 0903 03f0 26e8 a868 2100 fff7 b3ff  ......&..h!.....
-000018a0: 70bd f0b5 0606 0124 6048 9c46 2300 0768  p......$`H.F#..h
-000018b0: 360e 0ae0 1800 a040 1042 05d0 5c4d e001  6......@.B..\M..
-000018c0: 4019 3825 2e54 0163 641c bc42 f2d3 5649  @.8%.T.cd..B..VI
+00001880: 0006 03f0 e6ec 6c4d 0f22 c035 0721 a868  ......lM.".5.!.h
+00001890: 1202 0903 03f0 dcec a868 2100 fff7 b3ff  .........h!.....
+000018a0: 70bd f0b5 0606 0124 6148 9c46 2300 0768  p......$aH.F#..h
+000018b0: 360e 0ae0 1800 a040 1042 05d0 5d4d e001  6......@.B..]M..
+000018c0: 4019 3825 2e54 0163 641c bc42 f2d3 5749  @.8%.T.cd..B..WI
 000018d0: 6046 4018 7121 4906 8860 f0bd f8b5 0500  `F@.q!I..`......
-000018e0: e900 544e c036 706a 4418 6078 0028 18d1  ..TN.6pjD.`x.(..
-000018f0: 504f 0122 4037 f868 2900 03f0 0fff b868  PO."@7.h)......h
-00001900: 0122 2900 03f0 0aff 3069 0122 2900 03f0  .").....0i.")...
-00001910: 05ff 0121 2800 03f0 01fa 0020 2070 0120  ...!(......  p. 
+000018e0: e900 554e c036 706a 4418 6078 0028 18d1  ..UN.6pjD.`x.(..
+000018f0: 514f 0122 4037 f868 2900 04f0 61fc b868  QO."@7.h)...a..h
+00001900: 0122 2900 04f0 5cfc 3069 0122 2900 04f0  .")...\.0i.")...
+00001910: 57fc 0121 2800 03f0 f3fe 0020 2070 0120  W..!(......  p. 
 00001920: 6070 f8bd 70b5 0500 0800 0021 fff7 26ff  `p..p......!..&.
-00001930: 404c 0f22 c034 0721 a068 1202 0903 02f0  @L.".4.!.h......
-00001940: d2ef a068 2900 fff7 5eff 70bd f3b5 81b0  ...h)...^.p.....
-00001950: 0500 0021 0298 fff7 11ff 0124 364f 2600  ...!.......$6O&.
-00001960: 07e0 3000 a040 2842 02d0 385d fff7 b6ff  ..0..@(B..8]....
-00001970: 641c 2e48 0068 8442 f3d3 0299 2800 fff7  d..H.h.B....(...
-00001980: d1ff febd 10b5 0400 0800 0021 fff7 f6fe  ...........!....
-00001990: 0022 0121 2000 fff7 0dff 10bd f8b5 0103  .".! ...........
-000019a0: 0d0f 0104 090e 0006 8e46 204b 000e 0021  .........F K...!
-000019b0: 0a00 8446 1f68 0120 0fe0 1f4e 7346 365c  ...F.h. ...NsF6\
-000019c0: 0124 1e40 6645 00d0 0024 2600 8640 3143  .$.@fE...$&..@1C
-000019d0: 1b4e 365c b440 2243 401c b842 edd3 7126  .N6\.@"C@..B..q&
-000019e0: 1648 114c 2b00 7606 02f0 b8ef 0e08 0a0c  .H.L+.v.........
-000019f0: 1711 1317 1717 1717 1717 1710 1148 02e0  .............H..
-00001a00: 1148 00e0 1148 0023 03f0 36f8 f8bd c161  .H...H.#..6....a
-00001a10: 00e0 8161 1019 b060 f8bd 1300 0a00 2900  ...a...`......).
-00001a20: 0320 fff7 3eff f8bd 0000 c05e e400 4000  . ..>......^..@.
-00001a30: 0070 00e5 007f 00e5 2c07 4000 4000 00e2  .p......,.@.@...
-00001a40: 4007 4000 2509 0000 8509 0000 4d09 0000  @.@.%.......M...
-00001a50: 0a00 0100 2120 4004 10b5 02f0 58ed 0028  ....! @.....X..(
-00001a60: 03d1 ff49 c86a 401c c862 10bd 0243 70b5  ...I.j@..b...Cp.
-00001a70: 0d00 1400 1000 02f0 6eee 0121 0904 2043  ........n..!.. C
-00001a80: 6a18 0100 2120 4004 02f0 40ed 0028 03d1  j...! @...@..(..
-00001a90: f349 c86a 401c c862 70bd 70b5 0500 f14c  .I.j@..bp.p....L
-00001aa0: aa02 d60f 2279 c002 c00e 022a 16d1 a279  ...."y.....*...y
-00001ab0: 8242 13d1 2069 8842 10d1 216a e069 03f0  .B.. i.B..!j.i..
-00001ac0: a5fe 607a b042 06d0 6672 2078 6169 4200  ..`z.B..fr xaiB.
-00001ad0: 8018 0818 6061 0120 a581 a072 70bd 70b5  ....`a. ...rp.p.
-00001ae0: 0500 e04c 0e00 2179 c002 c00e 0229 0ed1  ...L..!y.....)..
-00001af0: a179 8142 0bd1 2069 b042 08d1 216a e069  .y.B.. i.B..!j.i
-00001b00: 03f0 84fe 0020 a081 2071 0320 a072 2a02  ..... .. q. .r*.
-00001b10: 0520 120a 3100 0006 fff7 a8ff 70bd d049  . ..1.......p..I
-00001b20: 4a68 521c 4a60 0021 8181 0121 c170 0221  JhR.J`.!...!.p.!
-00001b30: 8172 8e21 0172 7047 8172 c949 086b 401c  .r.!.rpG.r.I.k@.
-00001b40: 0863 7047 f3b5 4022 83b0 0d1d 087a 8e88  .cpG..@".....z..
-00001b50: 1043 0872 c34c 0020 c880 a079 c249 401c  .C.r.L. ...y.I@.
-00001b60: c006 c00e a071 497b 0022 4f07 7f0f 7901  .....qI{."O...y.
-00001b70: 0818 0290 311d 2800 fff7 d2ed c043 010a  ....1.(......C..
-00001b80: a970 0121 e870 0800 b840 0006 000e 2070  .p.!.p...@.... p
-00001b90: 0190 0020 6070 0398 2061 a81c 6061 a819  ... `p.. a..`a..
-00001ba0: 401c a061 0020 e070 6072 b048 2171 0068  @..a. .p`r.H!q.h
-00001bb0: e071 ab4d 8b20 2072 2869 401c 2861 0299  .q.M.  r(i@.(a..
-00001bc0: 3002 0026 4718 0020 a072 a948 0222 2100  0..&G.. .r.H."!.
-00001bd0: 02f0 f0fe 0028 e061 06d0 4169 2162 a349  .....(.a..Ai!b.I
-00001be0: 0969 03f0 45fe 05e0 ff22 5632 0020 a1a1  .i..E...."V2. ..
-00001bf0: 03f0 b2fd 0120 0399 3a00 0006 fff7 36ff  ..... ..:.....6.
-00001c00: a07a 0028 fcd0 a07a 0128 0cd1 207a 8028  .z.(...z.(.. z.(
-00001c10: 5bd1 0220 2071 0199 0120 8840 401e 0504  [..  q... .@@...
-00001c20: 2d0c a581 0ae0 a868 401c a860 e079 6862  -......h@..`.yhb
-00001c30: e079 0028 48d0 401e e071 c4e7 0026 20e0  .y.(H.@..q...& .
-00001c40: 6069 7100 7118 4718 e807 11d0 6079 617a  `iq.q.G.....`yaz
-00001c50: 4007 0907 4018 3106 4018 b978 0904 4018  @...@.1.@..x..@.
-00001c60: 7978 0902 4018 3978 4018 0399 fff7 f0fe  yx..@.9x@.......
-00001c70: a069 b842 02d8 0120 e070 05e0 6d08 03d0  .i.B... .p..m...
-00001c80: 761c 0198 8642 dbd3 0020 a072 0200 7c48  v....B... .r..|H
-00001c90: 2100 02f0 8ffe 0028 07d0 e061 4169 2162  !......(...aAi!b
-00001ca0: 7249 4969 03f0 e4fd 05e0 ff22 9c32 0020  rIIi.......".2. 
-00001cb0: 70a1 03f0 51fd a07a 0028 fcd0 e078 a589  p...Q..z.(...x..
-00001cc0: 0028 bbd0 002d b9d1 207a 05b0 f0bd 10b5  .(...-.. z......
-00001cd0: 0400 0078 0128 0bd1 6148 0168 491c 0160  ...x.(..aH.hI..`
-00001ce0: 2079 0028 05d1 a069 03f0 7afb 0020 2070   y.(...i..z..  p
-00001cf0: 10bd 401e 2071 a079 e178 4005 0904 4018  ..@. q.y.x@...@.
-00001d00: 2189 4218 0320 e168 0006 fff7 affe 5d48  !.B.. .h......]H
-00001d10: 0022 2100 02f0 4efe 0028 07d0 e061 4169  ."!...N..(...aAi
-00001d20: 2162 5249 8969 03f0 a3fd 10bd ff22 d332  !bRI.i.......".2
-00001d30: 0020 50a1 03f0 10fd 10bd c202 70b5 d40e  . P.........p...
-00001d40: 484a 0306 1579 1b0e 012d 11d1 9579 a542  HJ...y...-...y.B
-00001d50: 0ed1 1469 8c42 0bd1 8d2b 09d0 0002 400f  ...i.B...+....@.
-00001d60: 5071 0120 1372 9072 116a d069 03f0 4efd  Pq. .r.r.j.i..N.
-00001d70: 70bd f3b5 0102 0006 000e 83b0 090c c506  p...............
-00001d80: ed0e 0291 4109 0190 0120 8840 0090 0299  ....A.... .@....
-00001d90: ff20 1930 8142 02d8 0098 1028 0bd9 2a04  . .0.B.....(..*.
-00001da0: 0120 0499 8c32 4006 fff7 60fe 2c49 086a  . ...2@...`.,I.j
-00001db0: 401c 0862 89e7 2b4c 0826 2434 0027 2078  @..b..+L.&$4.' x
-00001dc0: 0128 23d1 e068 0499 8842 22d1 e078 a842  .(#..h...B"..x.B
-00001dd0: 1fd1 216a e069 03f0 19fd 2148 816a 491c  ..!j.i....!H.jI.
-00001de0: 8162 2804 b905 4218 0120 0499 8032 4006  .b(...B.. ...2@.
-00001df0: fff7 3cfe 1d4d 0022 6868 2071 2148 2100  ..<..M."hh q!H!.
-00001e00: 02f0 d8fd 0028 7bd1 1f4a 82e0 0028 00d1  .....({..J...(..
-00001e10: 3e00 2434 7f1c 082f d1d3 082e 0ad1 2a04  >.$4.../......*.
-00001e20: 0499 8d32 b005 fff7 21fe 0d49 8869 401c  ...2....!..I.i@.
-00001e30: 8861 4ae7 2420 0b49 7043 2431 4418 03f0  .aJ.$ .IpC$1D...
-00001e40: dffa 0028 22d1 2a04 0120 0499 8d32 4006  ...(".*.. ...2@.
-00001e50: fff7 0cfe 0249 c869 401c c861 35e7 0000  .....I.i@..a5...
-00001e60: 6c02 4000 2801 4000 007f 00e5 0000 4000  l.@.(.@.......@.
-00001e70: 390b 0000 7363 616d 702d 7032 702e 6300  9...scamp-p2p.c.
-00001e80: 1f0b 0000 cf0c 0000 2602 0000 0121 a061  ........&....!.a
-00001e90: 2170 019a 6271 049a e260 e570 009a 6270  !p..bq...`.p..bp
-00001ea0: 0022 a270 a271 009a 9140 491e 6181 801d  .".p.q...@I.a...
-00001eb0: 2181 2061 0299 4118 491e 6161 0299 2038  !. a..A.I.aa.. 8
-00001ec0: 8177 0299 090a c177 2804 7105 4218 0120  .w.....w(.q.B.. 
-00001ed0: 0499 8032 4006 fff7 c9fd 8d4d 8d49 6868  ...2@......M.Ihh
-00001ee0: 2071 b000 4018 026c 521c 0264 4869 0022   q..@..lR..dHi."
-00001ef0: 401c 4861 8848 2100 02f0 5cfd 0028 06d0  @.Ha.H!...\..(..
-00001f00: e061 4169 2162 a969 03f0 b2fc dde6 2722  .aAi!b.i......'"
-00001f10: 1201 8249 0020 03f0 1ffc d6e6 70b5 0400  ...I. ......p...
-00001f20: 7c48 0d00 c168 491c c160 2079 0028 05d1  |H...hI..` y.(..
-00001f30: a069 03f0 55fa 0020 2070 70bd 401e 2071  .i..U..  pp.@. q
-00001f40: e178 6805 0904 4218 0120 e168 8006 fff7  .xh...B.. .h....
-00001f50: 8dfd 7348 2a00 2100 02f0 2cfd 0028 07d0  ..sH*.!...,..(..
-00001f60: e061 4169 2162 6a49 c969 03f0 81fc 70bd  .aAi!bjI.i....p.
-00001f70: 6c4a 6a49 0020 03f0 effb 70bd 0202 520f  lJjI. ....p...R.
-00001f80: 2423 5a43 684b 10b5 d418 2278 c002 c00e  $#ZChK...."x....
-00001f90: 022a 0fd1 e278 8242 0cd1 e068 8842 09d1  .*...x.B...h.B..
-00001fa0: 0020 2070 216a e069 03f0 30fc a069 0021  .  p!j.i..0..i.!
-00001fb0: 01f0 fcfd 10bd f8b5 2423 460f 7343 5a4c  ........$#F.sCZL
-00001fc0: c200 1c19 2378 d20f 012b 6cd1 e368 8b42  ....#x...+l..h.B
-00001fd0: 69d1 a179 9142 66d1 6178 020e 491e 0a40  i..y.Bf.ax..I..@
-00001fe0: 2169 5300 d318 c918 030a 0870 000c 4b70  !iS........p..Kp
-00001ff0: 0127 8870 3800 9040 2289 8243 2281 6269  .'.p8..@"..C".bi
-00002000: 8a42 04d8 2189 401e 0140 2181 a770 2089  .B..!.@..@!..p .
-00002010: 0028 48d1 216a e069 03f0 f8fb a078 3c4d  .(H.!j.i.....x<M
-00002020: 0028 1bd0 0220 2070 e868 2071 e178 7005  .(...  p.h q.xp.
-00002030: 0904 4218 0120 e168 8006 fff7 17fd 3848  ..B.. .h......8H
-00002040: 3200 2100 02f0 b6fc 0028 04d0 e061 4169  2.!......(...aAi
-00002050: 2162 e969 25e0 334a 5032 27e0 a079 7840  !b.i%.3JP2'..yx@
-00002060: a071 6178 2269 4b00 c918 5118 2161 6189  .qax"iK...Q.!aa.
-00002070: 2181 e178 4005 0904 4018 2189 4218 0320  !..x@...@.!.B.. 
-00002080: e168 0006 fff7 f2fc a868 2071 2248 0022  .h.......h q"H."
-00002090: 2100 02f0 8ffc 0028 06d0 e061 4169 2162  !......(...aAi!b
-000020a0: a969 03f0 e5fb f8bd 1e4a 6832 1b49 0020  .i.......Jh2.I. 
-000020b0: 03f0 52fb f8bd 70b5 0400 0d00 02f0 4aeb  ..R...p.......J.
-000020c0: 0028 07d1 2001 000f 0128 04d1 2900 2000  .(.. ....(..). .
-000020d0: fff7 4ffe 70bd 0228 04d1 2900 2000 fff7  ..O.p..(..). ...
-000020e0: 2cfe 70bd 0328 04d1 2900 2000 fff7 d5fc  ,.p..(..). .....
-000020f0: 70bd 0428 04d1 2900 2000 fff7 f0fc 70bd  p..(..). .....p.
-00002100: 0528 fcd1 2900 2000 fff7 38ff 70bd 0000  .(..). ...8.p...
-00002110: 0000 4000 6c02 4000 cf0c 0000 740e 0000  ..@.l.@.....t...
-00002120: 1d0f 0000 9602 0000 4c01 4000 70b5 0500  ........L.@.p...
-00002130: 00e0 0c3d 0c2d fcda 0c00 00e0 0c3c 0c2c  ...=.-.......<.,
-00002140: fcda 0c26 7443 ff4e a419 655d 2c09 2d07  ...&tC.N..e],.-.
-00002150: 2d0f 001b 00d5 8018 491b 00d5 c918 0002  -.......I.......
-00002160: 2202 4018 f84b f849 5219 a039 da83 8880  ".@..K.IR..9....
-00002170: 0881 70bd f0b5 030a 0406 240e 0020 0626  ..p.......$.. .&
-00002180: 4100 711a 0422 8a40 521e 1d00 cd40 ad07  A.q..".@R....@..
-00002190: ad0f 2700 cf40 b907 090f 6d18 d243 1900  ..'..@....m..C..
-000021a0: 1140 2240 1218 0906 1204 8918 0122 aa40  .@"@.........".@
-000021b0: 8918 8201 e54d 401c 0428 a950 e0d3 f0bd  .....M@..(.P....
-000021c0: f0b5 89b0 0027 e149 b801 0890 0858 e049  .....'.I.....X.I
-000021d0: 000c 0840 0590 7900 0620 411a 0120 8840  ...@..y.. A.. .@
-000021e0: 401e 0026 0491 0390 0025 3002 0790 a800  @..&.....%0.....
-000021f0: 8019 0290 0798 0499 4019 8840 0599 0024  ........@..@...$
-00002200: 0818 0690 0399 e007 c00f 4843 039a 6108  ..........HC..a.
-00002210: 5143 069a 0002 1018 4018 0190 02f0 5afe  QC......@.....Z.
-00002220: 0628 0dd0 c94a 0898 0199 8018 029a 5200  .(...J........R.
-00002230: 8218 1182 029a 0121 8018 2030 0174 04e0  .......!.. 0.t..
-00002240: 032f 02d0 641c 042c dcd3 6d1c 042d ced3  ./..d..,..m..-..
-00002250: 761c 042e c8d3 7f1c 042f b4d3 09b0 f0bd  v......../......
-00002260: 10b5 bc4c 2379 012b 04d0 2300 0833 07c3  ...L#y.+..#..3..
-00002270: 0120 2071 10bd 10b5 b64c 1434 2379 012b  .  q.....L.4#y.+
-00002280: 04d0 2300 0833 07c3 0120 2071 10bd ffb5  ..#..3...  q....
-00002290: 81b0 0500 1600 af4c 0020 2071 8804 0521  .......L.  q...!
-000022a0: 4905 4018 2a00 0021 02f0 30e9 0028 02d1  I.@.*..!..0..(..
-000022b0: 8f20 05b0 f0bd a848 0222 211d 02f0 7afb  . .....H."!...z.
-000022c0: 0500 05d1 ff22 a5a1 03f0 46fa 8a20 f0e7  ....."....F.. ..
-000022d0: 6f69 0499 2800 03f0 cbfa 2079 0028 fcd0  oi..(..... y.(..
-000022e0: 2079 0228 01d1 8620 e3e7 3900 2800 03f0   y.(... ..9.(...
-000022f0: 8dfa 002e 01d0 e068 3060 8020 d9e7 f8b5  .......h0`. ....
-00002300: 0500 0800 934c 1f00 0021 1434 2171 1168  .....L...!.4!q.h
-00002310: 5122 8004 5204 8018 2a00 02f0 f8e8 0028  Q"..R...*......(
-00002320: 01d1 8f20 f8bd 8c48 0222 211d 02f0 42fb  ... ...H."!...B.
-00002330: 0500 06d1 ff22 2232 88a1 03f0 0dfa 8a20  .....""2....... 
-00002340: f8bd 6e69 3900 2800 03f0 92fa 2279 002a  ..ni9.(....."y.*
-00002350: fcd0 2079 0228 01d1 8620 f8bd 3100 2800  .. y.(... ..1.(.
-00002360: 03f0 54fa 8020 f8bd f3b5 81b0 0025 0700  ..T.. .......%..
-00002370: 2c00 0126 a640 3800 3042 16d0 7120 029b  ,..&.@8.0B..q ..
-00002380: 0022 2100 4006 fff7 82ff 0028 0dd0 7148  ."!.@......(..qH
-00002390: 754a 0169 9142 08d1 c168 744a 090d 9142  uJ.i.B...htJ...B
-000023a0: 03d1 8068 a042 00d1 3543 641c 062c e0d3  ...h.B..5Cd..,..
-000023b0: 3806 04d5 6e48 0560 6348 a038 0573 2800  8...nH.`cH.8.s(.
-000023c0: febd 604a 203a 1068 0028 08d0 0168 1160  ..`J :.h.(...h.`
-000023d0: 5168 491c 5160 9368 9942 00d9 9160 7047  QhI.Q`.h.B...`pG
-000023e0: 5849 2039 0a68 0260 0860 4868 401e 4860  XI 9.h.`.`Hh@.H`
-000023f0: 7047 5549 a039 c879 401c 7f28 00d9 0120  pGUI.9.y@..(... 
-00002400: c871 4000 7047 0006 410e 4809 c906 c90e  .q@.pG..A.H.....
-00002410: 0122 8a40 8100 10b5 564c 801c 0919 4b6a  .".@....VL....Kj
-00002420: 8007 1343 4b62 0021 000f 0019 4162 10bd  ...CKb.!....Ab..
-00002430: ffb5 81b0 0400 002b 02d0 fff7 daff 0443  .......+.......C
-00002440: f820 1040 5507 0090 0299 6d0f 160a 2000  . .@U.....m... .
-00002450: 02f0 7ce9 2043 0127 0190 0024 4449 3800  ..|. C.'...$DI8.
-00002460: a040 0968 3040 0842 0ad0 0098 02f0 88f9  .@.h0@.B........
-00002470: 4121 a004 4904 4018 019a 0299 02f0 46e8  A!..I.@.......F.
-00002480: 641c 062c ead3 6d1e e7d2 12e7 2e48 3949  d..,..m......H9I
-00002490: 8038 007a 8870 2c48 2a49 2030 8069 2039  .8.z.p,H*I 0.i 9
-000024a0: c860 3548 0860 0021 0b00 1a00 0f29 01d0  .`5H.`.!.....)..
-000024b0: 0200 1432 0260 1430 491c 1029 f5d3 7047  ...2.`.0I..)..pG
-000024c0: f8b5 0500 0804 000c 0e00 0706 040a 3f0e  ..............?.
-000024d0: 2900 02f0 27fd 2948 360c 4057 3306 0419  )...'.)H6.@W3...
-000024e0: 2648 320a 0830 4057 1b0e c519 d018 2449  &H2..0@W......$I
-000024f0: 4000 401f 0860 2348 134f 0660 a03f 2249  @.@..`#H.O.`.?"I
-00002500: 0120 7e80 0860 9442 b871 01db 0024 02e0  . ~..`.B.q...$..
-00002510: 002c 00da a418 9d42 01db 0025 02e0 002d  .,.....B...%...-
-00002520: 00da ed18 2900 2000 fff7 00fe 2002 4019  ....). ..... .@.
-00002530: 164c 0721 0906 4118 0122 2060 5207 3880  .L.!..A.." `R.8.
-00002540: 9161 25e0 4000 4000 a07f 00e5 2c04 4000  .a%.@.@.....,.@.
-00002550: fcfc 0000 0407 4000 4729 0000 7363 616d  ......@.G)..scam
-00002560: 702d 6e6e 2e63 0000 0100 00e2 9105 0000  p-nn.c..........
-00002570: 2401 4000 2c05 4000 ec02 4000 3449 0000  $.@.,.@...@.4I..
-00002580: 2001 4000 1c01 4000 ec00 4000 e800 4000   .@...@...@...@.
-00002590: 0721 02f0 c7fc 2068 fff7 ecfd 2168 0120  .!.... h....!h. 
-000025a0: c007 8900 ff4a d268 5050 2168 3004 4018  .....J.hPP!h0.@.
-000025b0: f8bd 0022 1100 8306 10b5 03d5 010e 0906  ..."............
-000025c0: ff22 1206 c306 05d5 ff24 2404 0300 2340  .".......$$...#@
-000025d0: 1943 2243 0307 05d5 0124 e403 0300 2340  .C"C.....$....#@
-000025e0: 1943 2243 4307 05d5 1f24 2402 0300 2340  .C"CC....$$...#@
-000025f0: 1943 2243 8307 03d5 c023 1840 0143 1a43  .C"C.....#.@.C.C
-00002600: e123 1b06 1868 9043 0843 1860 10bd e64a  .#...h.C.C.`...J
-00002610: 030f 10b5 02f0 a2e9 0604 0b0e 1627 2e30  .............'.0
-00002620: e24b 010a 1972 9170 5872 d070 24e0 02f0  .K...r.pXr.p$...
-00002630: adfe 21e0 0107 dd48 090f 2038 c173 0021  ..!....H.. 8.s.!
-00002640: 0162 19e0 1169 8142 01d1 0020 10bd 1061  .b...i.B... ...a
-00002650: c007 01d0 ff21 00e0 0021 d348 1022 2430  .....!...!.H."$0
-00002660: 02f0 6ae9 08e0 0022 d148 1100 1300 02f0  ..j....".H......
-00002670: 03fa 01e0 fff7 92f9 0120 10bd 0a03 10b5  ......... ......
-00002680: 940f 8a03 930f c94a 203a 012b 02d1 e522  .......J :.+..."
-00002690: 1206 09e0 022b 02d1 7122 5206 04e0 032b  .....+..q"R....+
-000026a0: 02d1 c24a 2032 126a 0904 090e 8918 002c  ...J 2.j.......,
-000026b0: 01d1 0870 10bd 012c 01d1 0880 10bd 0860  ...p...,.......`
-000026c0: 10bd 0a02 120f 00d1 d8e7 7047 f7b5 0300  ..........pG....
-000026d0: 0c00 080c b34a 8d05 d268 8100 82b0 8e46  .....J...h.....F
-000026e0: 0192 5158 0127 0a0e 9446 b24a 0904 1268  ..QX.'...F.J...h
-000026f0: bf02 2600 ad0d 090c 3e43 9042 17d0 6345  ..&.....>C.B..cE
-00002700: 01d1 8d42 13d2 ac4a 9142 04d1 a74a c032  ...B...J.B...J.2
-00002710: 5188 491c 5180 1906 019b 4a19 7146 5a50  Q.I.Q.....J.qFZP
-00002720: 0499 02f0 fffb a548 0068 8542 00d3 3400  .......H.h.B..4.
-00002730: 601c bee5 9d4a 70b5 a032 9b4c 9268 e261  `....Jp..2.L.h.a
-00002740: a061 0802 400e 2071 080a 6071 0020 a071  .a..@. q..`q. .q
-00002750: 6072 0100 6070 2000 2022 3430 02f0 ece8  `r..`p . "40....
-00002760: 2000 2022 0021 7430 02f0 e6e8 a169 0123   . ".!t0.....i.#
-00002770: 0804 090c 8a07 000c 920f 0028 08d0 9501  ...........(....
-00002780: e21f f93a 5259 150c 8d42 02d1 0242 00d0  ...:RY...B...B..
-00002790: 6372 2370 70bd f8b5 834c 2379 8342 0fd1  cr#pp....L#y.B..
-000027a0: 2078 0128 0cd1 1002 000e 4509 c606 f60e   x.(......E.....
-000027b0: 0123 b340 ad00 2e19 756b 2f00 1f42 01d0  .#.@....uk/..B..
-000027c0: 0020 f8bd 1d43 7563 2162 6161 1104 090e  . ...Cuc!baa....
-000027d0: 491c a181 e071 0020 0100 e081 7248 2022  I....q. ....rH "
-000027e0: 5430 02f0 aae8 0220 2070 0120 f8bd 1302  T0.....  p. ....
-000027f0: 70b5 1c0e 6c4b 1d79 8542 12d1 d879 a042  p...lK.y.B...y.B
-00002800: 0fd1 1878 0228 0cd1 1004 000e 4409 c506  ...x.(......D...
-00002810: ed0e 0122 aa40 a400 e518 6c6d 2600 1642  ...".@....lm&..B
-00002820: 01d0 0020 70bd de89 8000 761c 1443 c018  ... p.....v..C..
-00002830: de81 c030 6c65 8161 5869 4018 5861 0120  ...0le.aXi@.Xa. 
-00002840: 70bd 70b5 1202 584d 120e 2b79 8342 11d1  p.p...XM..+y.B..
-00002850: e879 9042 0ed1 2878 0228 0bd1 5009 d206  .y.B..(x.(..P...
-00002860: 0126 d20e 3400 9440 8000 4219 506f 0300  .&..4..@..B.Po..
-00002870: 2342 01d0 0020 70bd 2043 5067 6869 4018  #B... p. CPghi@.
-00002880: 6861 0dd1 e989 a889 8142 09d1 a979 8200  ha.......B...y..
-00002890: 491c a971 4449 286a d831 02f0 24e8 00e0  I..qDI(j.1..$...
-000028a0: 6e70 0120 2e70 70bd 0a00 3f49 10b5 0b79  np. .pp...?I...y
-000028b0: 8342 02d1 0878 0128 01d0 0020 10bd 0020  .B...x.(... ... 
-000028c0: 0870 4878 0028 11d1 8b79 4879 8342 0dd1  .pHx.(...yHy.B..
-000028d0: 487a 0028 0ad0 c969 3948 0023 02f0 ccf8  Hz.(...i9H.#....
-000028e0: 0028 03d1 374a 3849 02f0 36ff 0120 10bd  .(..7J8I..6.. ..
-000028f0: f3b5 81b0 0500 0027 4679 c079 7106 00d4  .......'Fy.yq...
-00002900: 0700 0024 0121 0800 a040 3042 16d0 e019  ...$.!...@0B....
-00002910: 0628 00d3 801f 2d4a 8140 1268 1142 0dd0  .(....-J.@.h.B..
-00002920: a968 8004 0818 2a69 e968 01f0 f0ed 0028  .h....*i.h.....(
-00002930: 04d1 244a 2449 1b32 02f0 0eff 641c 062c  ..$J$I.2....d..,
-00002940: e0d3 029a 521e 0cd0 ab79 2148 2900 02f0  ....R....y!H)...
-00002950: c7ff 0028 04d1 3322 1b49 1201 02f0 fcfe  ...(..3".I......
-00002960: febd 2800 fff7 3cfd febd 70b5 0c04 0f4b  ..(...<...p....K
-00002970: 0c4d a033 ee69 5a68 2418 b600 9451 ee69  .M.3.iZh$....Q.i
-00002980: 0024 761c ee61 b600 9451 0404 d86b 240c  .$v..a...Q...k$.
-00002990: 401c d863 0126 3000 2a69 8840 002a 20d1  @..c.&0.*i.@.* .
-000029a0: 2c61 17e0 2000 4000 2c05 4000 207f 00e5  ,a.. .@.,.@. ...
-000029b0: c111 0000 e800 4000 ffff 0000 2001 4000  ......@..... .@.
-000029c0: 0708 0000 0b03 0000 5c15 0000 2401 4000  ........\...$.@.
-000029d0: f118 0000 704a 5c63 1268 8243 6a61 9a63  ....pJ\c.h.Cja.c
-000029e0: 0ae0 a242 0ad9 2c61 5c63 6a69 8243 a869  ...B..,a\cji.C.i
-000029f0: 8640 1643 6e61 9e63 a961 05e0 6969 0124  .@.Cna.c.a..ii.$
-00002a00: 8143 6961 e407 9963 6b69 0022 6349 4033  .Cia...cki."cI@3
-00002a10: d243 0020 02f0 20fa 601c 70bd f7b5 1000  .C. .. .`.p.....
-00002a20: 0c00 1600 01f0 92ee 0028 04d0 5c48 4169  .........(..\HAi
-00002a30: 491c 4161 febd 3001 5949 050f aa00 c039  I.Aa..0.YI.....9
-00002a40: 5118 8031 4a69 3006 521c 400e 082d 4a61  Q..1Ji0.R.@..-Ja
-00002a50: 1ad2 0028 18d0 4309 c206 d20e 0121 9140  ...(..C......!.@
-00002a60: 4f4f 9a00 c03f d219 9446 526a 1700 0f42  OO...?...FRj...B
-00002a70: e0d1 0a43 6746 9b1c 7a62 4949 9a07 c039  ...CgF..zbII...9
-00002a80: 0023 120f 5118 4b62 2b00 01f0 68ef 100a  .#..Q.Kb+...h...
-00002a90: 0e12 091c 2127 092c 3409 093b 4045 4a09  ....!'.,4..;@EJ.
-00002aa0: c8e7 2000 fff7 b3fd 3fe0 2000 fff7 81fd  .. .....?. .....
-00002ab0: 3de0 3c49 086a 801c a042 bbd8 6040 b9d4  =.<I.j...B..`@..
-00002ac0: 601e 0862 33e0 3100 2000 fff7 fafd 2ee0  `..b3.1. .......
-00002ad0: 0098 2100 fff7 f4fc 0400 28e0 3100 2000  ..!.......(.1. .
-00002ae0: fff7 28fe 23e0 009a 2100 fff7 effd 0400  ..(.#...!.......
-00002af0: 4005 9fd4 1be0 0099 2000 fff7 36ff 041e  @....... ...6...
-00002b00: 98db 14e0 3200 2100 fff7 45fe 0de0 3200  ....2.!...E...2.
-00002b10: 2100 fff7 6cfe 08e0 3200 2100 fff7 91fe  !...l...2.!.....
-00002b20: 03e0 3200 2100 fff7 bffe 0028 82d0 6807  ..2.!......(..h.
-00002b30: 04d5 1b48 c038 8778 c578 03e0 3002 070e  ...H.8.x.x..0...
-00002b40: 3004 050e 3601 3609 2100 3000 01f0 feed  0...6.6.!.0.....
-00002b50: 0643 fff7 36fc 0028 01d1 134a 17e0 f821  .C..6..(...J...!
-00002b60: 2940 0831 4771 8171 0099 c171 0f49 0823  )@.1Gq.q...q.I.#
-00002b70: 0a68 0661 c460 8260 6a07 520f 0100 0c48  .h.a.`.`j.R....H
-00002b80: 521c 02f0 adfe 0028 8ad1 7d22 d200 0949  R......(..}"...I
-00002b90: 0020 02f0 e1fd febd 2401 4000 5555 ffff  . ......$.@.UU..
-00002ba0: ec05 4000 007f 00e5 db03 0000 4449 0000  ..@.........DI..
-00002bb0: f118 0000 5c15 0000 10b5 c269 8169 d30f  ....\......i.i..
-00002bc0: 4069 db07 fff7 34fc 0020 10bd f0b5 0600  @i....4.. ......
-00002bd0: 85b0 4169 0023 080c 0390 fe20 0140 0291  ..Ai.#..... .@..
-00002be0: fa49 b069 f769 0840 0299 039a 4018 0321  .I.i.i.@....@..!
-00002bf0: 8906 4018 3900 fff7 1bfc b069 3500 0104  ..@.9......i5...
-00002c00: 090e 491c 0091 ff21 0904 0840 0299 4018  ..I....!...@..@.
-00002c10: 0d21 0906 4018 2035 0024 0190 09e0 019a  .!..@. 5.$......
-00002c20: 02cd 2002 8018 039a 7f18 0023 fff7 00fc  .. ........#....
-00002c30: 641c 0098 8442 f2d3 b069 ff21 0904 0840  d....B...i.!...@
-00002c40: 0299 039a 4018 0721 4906 4018 7942 0023  ....@..!I.@.yB.#
-00002c50: fff7 eefb 0020 05b0 f0bd f3b5 0400 8422  ..... ........."
-00002c60: 81b0 4169 0802 0e06 000e 360e 0428 01d8  ..Ai......6..(..
-00002c70: 102e 01d3 2282 6ce0 d54d 0028 02d0 0128  ....".l..M.(...(
-00002c80: 45d1 02e0 00f0 2afe 0600 ff2e 35d0 7001  E.....*.....5.p.
-00002c90: 4519 2022 0021 2800 01f0 4eee 6169 0801  E. ".!(...N.ai..
-00002ca0: 090d 0f0a 000f 3f02 0028 02d0 411e 0120  ......?..(..A.. 
-00002cb0: 8840 0743 a881 ef81 a069 000c e882 6069  .@.C.....i....`i
-00002cc0: 000a 2876 e069 0028 07d0 2000 1c30 2900  ..(v.i.(.. ..0).
-00002cd0: fef7 96fb b805 06d5 11e0 b805 0fd4 2900  ..............).
-00002ce0: 02a8 fef7 8dfb a069 6881 e889 0121 4903  .......ih....!I.
-00002cf0: 0843 e881 2800 fef7 28fc 6661 23e0 a069  .C..(...(.fa#..i
-00002d00: a882 e889 0121 c903 0843 e881 f5e7 0228  .....!...C.....(
-00002d10: 0ed1 7001 4119 a069 4501 ff20 0130 8542  ..p.A..iE.. .0.B
-00002d20: a8d8 2000 2a00 1430 01f0 88ed 2800 febd  .. .*..0....(...
-00002d30: 0428 0ad1 a749 a84a 0868 8018 6061 a069  .(...I.J.h..`a.i
-00002d40: 1028 00d2 0860 0420 febd 0020 7101 4919  .(...`. ... q.I.
-00002d50: c881 0020 febd a149 10b5 0988 0a04 a049  ... ...I.......I
-00002d60: 4b68 0968 1b02 d218 5118 4161 9d49 8161  Kh.h....Q.Aa.I.a
-00002d70: 9d49 0968 c161 2030 9ca1 01f0 9eed 1c20  .I.h.a 0....... 
-00002d80: 10bd f0b5 0500 85b0 8069 0290 e869 0190  .........i...i..
-00002d90: 0298 ff21 0131 8842 02d8 0198 0528 01d9  ...!.1.B.....(..
-00002da0: 8420 13e0 8d48 2e00 1436 2030 807a 6f69  . ...H...6 0.zoi
-00002db0: 0090 0298 0024 8008 0390 0ee0 009b 0199  .....$..........
-00002dc0: 3200 3800 fff7 63fa 8028 02d0 2882 0020  2.8...c..(..(.. 
-00002dd0: 41e7 0398 3f1d 361d 641c a042 eed8 0298  A...?.6.d..B....
-00002de0: 39e7 feb5 0500 8069 e969 0191 ff21 0131  9......i.i...!.1
-00002df0: 8842 02d8 0199 0529 01d9 8420 12e0 7749  .B.....)... ..wI
-00002e00: 2e00 2036 2031 897a 6f69 0024 8008 0091  .. 6 1.zoi.$....
-00002e10: 0290 0de0 009b 0199 3200 3800 fff7 6ffa  ........2.8...o.
-00002e20: 8028 01d0 2882 05e0 0298 3f1d 361d 641c  .(..(.....?.6.d.
-00002e30: a042 efd8 0020 febd f8b5 0500 0e00 010c  .B... ..........
-00002e40: 0a06 080a 120e 8018 6c4a 4000 401f 1060  ........lJ@.@..`
-00002e50: 2804 000c 6a4c 0723 604a 1b06 c318 0127  (...jL.#`J.....'
-00002e60: 2060 7f07 1080 bb61 664b 1960 664b 5180   `.....afK.`fKQ.
-00002e70: 0121 1960 9171 0721 02f0 54f8 634a 2168  .!.`.q.!..T.cJ!h
-00002e80: 1268 b800 8900 5050 2068 fff7 73f9 fff7  .h....PP h..s...
-00002e90: b0fa 0400 fff7 b7fa 0520 0006 3200 2900  ......... ..2.).
-00002ea0: 2018 0023 fff7 c4fa f8bd 10b5 c169 8069   ..#.........i.i
-00002eb0: fff7 c2ff 0020 10bd 10b5 8169 4069 fef7  ..... .....i@i..
-00002ec0: a2fc 0020 10bd 10b5 4169 ca07 02d0 8421  ... ....Ai.....!
-00002ed0: 0182 04e0 4148 c030 8068 fef7 94fc 0020  ....AH.0.h..... 
-00002ee0: 10bd 70b5 0400 4269 1006 000e 110c 0028  ..p...Bi.......(
-00002ef0: 03d1 0120 01f0 74ff 11e0 8425 0128 03d1  ... ..t....%.(..
-00002f00: a069 01f0 41ff 07e0 0228 07d1 1004 030e  .i..A....(......
-00002f10: e269 a069 01f0 7eff 0028 00d1 2582 0020  .i.i..~..(..%.. 
-00002f20: 70bd 0243 70b5 0d00 1400 1000 01f0 12ec  p..Cp...........
-00002f30: 0121 2a00 4904 2043 0a43 0100 2120 4004  .!*.I. C.C..! @.
-00002f40: 01f0 e4ea 70bd f8b5 8202 0f00 0101 0323  ....p..........#
-00002f50: 9b06 890f 9843 4b1c 9b07 1e09 8b01 2c49  .....CK.......,I
-00002f60: 0643 0020 5d18 a880 e880 0120 920f 0004  .C. ]...... ....
-00002f70: 012a 00d0 0020 0024 e860 0120 a040 3842  .*... .$.`. .@8B
-00002f80: 11d0 2819 2030 007c 0028 0cd0 6000 2818  ..(. 0.|.(..`.(.
-00002f90: 018a a888 0322 401c a880 3000 9205 1040  ....."@...0....@
-00002fa0: 3200 fff7 beff 641c 102c e6d3 f8bd 0b00  2.....d..,......
-00002fb0: 1749 8201 5218 1189 d268 1b05 d218 3f23  .I..R....h....?#
-00002fc0: 8006 9b06 c018 1218 0020 aae7 00ff ff00  ......... ......
-00002fd0: 0c09 4000 e000 4000 0020 0808 007f 00e5  ..@...@.. ......
-00002fe0: 3c0b 4000 0001 8500 704d 0000 5343 264d  <.@.....pM..SC&M
-00002ff0: 502f 5370 694e 4e61 6b65 7200 2001 4000  P/SpiNNaker. .@.
-00003000: e800 4000 1c01 4000 ec00 4000 2c00 4000  ..@...@...@.,.@.
-00003010: 2c04 4000 f3b5 81b0 0600 01f0 9ceb 0028  ,.@............(
-00003020: 31d1 3101 8c0f b102 3002 8d0f cc49 800f  1.1.....0....I..
-00003030: 0028 29d1 3003 000b 002d 0bd1 a201 5218  .().0....-....R.
-00003040: d368 0504 2d0c 5b19 0125 2d04 2840 0343  .h..-.[..%-.(@.C
-00003050: d360 13e0 012d 0cd1 a201 5318 da68 0126  .`...-....S..h.&
-00003060: 1518 2d04 2d0c 3604 3040 0240 2a43 da60  ..-.-.6.0@.@*C.`
-00003070: 04e0 a201 5218 d368 1818 d060 a001 4018  ....R..h...`..@.
-00003080: c188 491c c180 febd 002c 15d0 a201 5118  ..I......,....Q.
-00003090: 0298 0881 3101 0022 b248 0909 d243 0523  ....1..".H...C.#
-000030a0: 02f0 1efc 0420 031b c820 4343 ae48 2a00  ..... ... CC.H*.
-000030b0: 2100 02f0 15fc febd 0124 0128 53d1 3006  !........$.(S.0.
-000030c0: 000e 8446 3004 000e 8646 3003 a74a 030f  ...F0....F0..J..
-000030d0: 0020 1268 0121 0ae0 a54e 7746 765c 0124  . .h.!...NwFv\.$
-000030e0: 3e40 6645 00d0 0024 8c40 2043 491c 9142  >@fE...$.@ CI..B
-000030f0: f2d3 a04f 0024 022d 0fd1 0121 0ae0 0126  ...O.$.-...!...&
-00003100: 8e40 0642 05d0 ce01 f619 b67b 9e42 00d1  .@.B.......{.B..
-00003110: 641c 491c 9142 f2d3 2ae0 002d 11d1 0121  d.I..B..*..-...!
-00003120: 0be0 0126 8e40 0642 06d0 ce01 f619 b67b  ...&.@.B.......{
-00003130: 9e42 01d1 0124 2404 491c 9142 f1d3 641c  .B...$$.I..B..d.
-00003140: 16e0 0124 2404 0121 0ae0 0126 8e40 0642  ...$$..!...&.@.B
-00003150: 05d0 ce01 f619 b67b 9e42 00d0 0024 491c  .......{.B...$I.
-00003160: 9142 f2d3 ebe7 0228 02d1 3000 fef7 16fc  .B.....(..0.....
-00003170: 2805 0321 0019 8906 4218 0299 0020 fff7  (..!....B.... ..
-00003180: d0fe febd 70b5 0400 4169 8069 0029 06d1  ....p...Ai.i.)..
-00003190: 0100 0120 784a 4004 01f0 b8e9 20e0 8422  ... xJ@..... .."
-000031a0: 0129 12d1 e169 0029 01d1 2282 18e0 0201  .)...i.)..".....
-000031b0: 950f fff7 c8fe 7148 01f0 e2fa 6849 a801  ......qH....hI..
-000031c0: 4018 c068 6061 0420 70bd 0229 edd1 0521  @..h`a. p..)...!
-000031d0: 3f22 0907 1202 4118 1002 0123 fff7 28f9  ?"....A....#..(.
-000031e0: 0020 70bd 70b5 0400 4069 0306 0004 1b0e  . p.p...@i......
-000031f0: 000e 052b 02d9 8420 2082 27e0 604d 01f0  ...+...  .'.`M..
-00003200: aeeb 0604 0c12 1b21 2719 0302 e269 a169  .......!'....i.i
-00003210: e868 db1c 02f0 dcf9 0be0 a169 e868 0122  .h.........i.h."
-00003220: 02f0 38fa 12e0 eb68 0100 0122 1800 02f0  ..8....h..."....
-00003230: 75fa 6061 0420 70bd a269 0100 1000 01f0  u.`a. p..i......
-00003240: bffc f6e7 e169 a069 01f0 12fd 0020 70bd  .....i.i..... p.
-00003250: a169 01f0 63fd ece7 70b5 8423 4169 8269  .i..c...p..#Ai.i
-00003260: 1229 01d9 0382 23e0 d207 04d0 444a 4032  .)....#.....DJ@2
-00003270: 8a18 127d 02e0 434c 0a00 615c 002a f1d0  ...}..CL..a\.*..
-00003280: 3a4c 2568 aa42 edd2 0120 8840 7121 4906  :L%h.B... .@q!I.
-00003290: 4861 3d48 4068 00f0 d4fd fef7 e6fa 2068  Ha=H@h........ h
-000032a0: 3449 c001 2039 4018 8022 0021 01f0 44eb  4I.. 9@..".!..D.
-000032b0: 0020 70bd 10b5 8288 182a 01d2 8121 4de0  . p......*...!M.
-000032c0: 038a 8022 0282 01f0 4aeb 1e10 4813 1648  ..."....J...H..H
-000032d0: 1948 4848 4848 4848 4848 483c 2427 3933  .HHHHHHHHHH<$'93
-000032e0: 3042 2a36 1c2d 213f 4548 fff7 34fd 10bd  0B*6.-!?EH..4...
-000032f0: 01f0 4cfe 10bd 01f0 9ffe 10bd 01f0 3ffe  ..L...........?.
-00003300: 10bd 4069 02f0 42f8 0020 10bd fdf7 caff  ..@i..B.. ......
-00003310: 10bd fff7 36fd 10bd fff7 63fd 10bd fff7  ....6.....c.....
-00003320: 55fc 10bd fff7 99fc 10bd fff7 befd 10bd  U...............
-00003330: fff7 42fc 10bd fff7 bffd 10bd fff7 c3fd  ..B.............
-00003340: 10bd fff7 89ff 10bd fff7 4cff 10bd fff7  ..........L.....
-00003350: 19ff 10bd fff7 c5fd 10bd 8321 0182 d3e7  ...........!....
-00003360: 2c04 4000 471f 0000 af1f 0000 e400 4000  ,.@.G.........@.
-00003370: 2c07 4000 2070 00e5 5555 ffff 1027 0000  ,.@. p..UU...'..
-00003380: 407f 00e5 4007 4000 3c0b 4000 0022 334b  @...@.@.<.@.."3K
-00003390: d243 10b5 07e0 0478 401c 5440 2406 a40d  .C.....x@.T@$...
-000033a0: 1c59 120a 6240 491e f5d2 d043 10bd 70b5  .Y..b@I....C..p.
-000033b0: 0500 0c00 01f0 cae9 2843 0122 0021 5207  ........(C.".!R.
-000033c0: 4125 6d04 1368 002b fcda 8b04 2b43 1360  A%m..h.+....+C.`
-000033d0: 5460 9060 491c 0629 f4d3 2148 8078 01f0  T`.`I..)..!H.x..
-000033e0: cff9 70bd f8b5 1f49 8872 1e49 0020 4031  ..p....I.r.I. @1
-000033f0: 0870 1b21 1c48 0904 fff7 d9ff 0025 1b48  .p.!.H.......%.H
-00003400: 2e04 a902 3043 0091 fff7 d1ff 0024 2f02  ....0C.......$/.
-00003410: 3000 2102 0843 1649 8122 0843 3919 8900  0.!..C.I.".C9...
-00003420: d203 8918 0968 fff7 c2ff 641c ff2c efd9  .....h....d..,..
-00003430: 1048 8121 0643 0098 c903 4018 0121 8902  .H.!.C....@..!..
-00003440: fff7 a4ff 0100 3000 fff7 b1ff 6d1c 1c2d  ......0.....m..-
-00003450: d5d3 0948 0021 fff7 aaff f8bd 5049 0000  ...H.!......PI..
-00003460: 407f 00e5 8081 4000 0300 0001 03ff 0002  @.....@.........
-00003470: 0300 0003 0300 0004 0301 0005 0f00 2de9  ..............-.
-00003480: 2403 9fe5 0232 a0e3 0110 d0e5 0110 81e2  $....2..........
-00003490: 1f10 01e2 0110 c0e5 8110 81e0 0111 80e0  ................
-000034a0: 0420 b1e5 0020 83e5 0208 12e3 0420 9115  . ... ....... ..
-000034b0: 0420 8315 0810 91e5 0810 83e5 0210 d0e5  . ..............
-000034c0: 0110 41e2 0210 c0e5 0210 d0e5 1f04 a0e3  ..A.............
-000034d0: 0000 51e3 021b a003 1410 8005 3000 80e5  ..Q.........0...
-000034e0: 0f00 bde8 04f0 5ee2 0f50 2de9 0212 a0e3  ......^..P-.....
-000034f0: 1000 91e5 1410 91e5 aa2c 81e2 ab20 92e2  .........,... ..
-00003500: 7504 000b 0f50 bde8 04f0 5ee2 0f50 2de9  u....P....^..P-.
-00003510: 0202 a0e3 0c30 90e5 1010 90e5 1420 90e5  .....0....... ..
-00003520: 8302 a0e1 0208 13e3 a00e a0e1 0130 02e2  .............0..
-00003530: 0500 000a 0000 53e3 0100 000a 47fb fffa  ......S.....G...
-00003540: 0300 00ea 34fd fffa 0100 00ea 0000 53e3  ....4.........S.
-00003550: 6304 001b 1f04 a0e3 3000 80e5 0f50 bde8  c.......0....P..
-00003560: 04f0 5ee2 0f50 2de9 0212 a0e3 1000 91e5  ..^..P-.........
-00003570: 1410 91e5 0127 a0e1 222f a0e1 0118 a0e1  .....'.."/......
-00003580: 0200 52e3 2118 a0e1 0100 001a a0fe fffa  ..R.!...........
-00003590: 0500 00ea 0000 52e3 0100 001a 84fa fffb  ......R.........
-000035a0: 0100 00ea 0100 52e3 4f04 000b 1f04 a0e3  ......R.O.......
-000035b0: 3000 80e5 0f50 bde8 04f0 5ee2 ff50 2de9  0....P....^..P-.
-000035c0: 2104 a0e3 0c00 80e5 e041 9fe5 d000 c4e1  !........A......
-000035d0: 1060 44e2 0100 90e2 0010 a1e2 f000 c4e1  .`D.............
-000035e0: b801 d6e1 0f5c 46e2 0140 80e2 fa0f 54e3  .....\F..@....T.
-000035f0: 0c00 001a 1c0f 95e5 0040 a0e3 0100 80e2  .........@......
-00003600: 1c0f 85e5 a801 9fe5 0230 a0e3 0420 a0e1  .........0... ..
-00003610: 0410 a0e1 1705 00fa 0000 50e3 e620 a003  ..........P.. ..
-00003620: 191e 8f02 4908 000b b841 c6e1 9061 9fe5  ....I....A...a..
-00003630: 0000 96e5 0140 80e2 0a00 54e3 0900 001a  .....@....T.....
-00003640: 0040 a0e3 7c01 9fe5 0130 a0e3 0420 a0e1  .@..|....0... ..
-00003650: 0410 a0e1 0705 00fa 0000 50e3 f220 a003  ..........P.. ..
-00003660: 151e 8f02 3908 000b 0040 86e5 0f1f d5e5  ....9....@......
-00003670: 0000 51e3 0900 000a 200f 95e5 0100 80e2  ..Q..... .......
-00003680: 200f 85e5 3001 a0e1 e114 a0e3 0020 91e5   ...0........ ..
-00003690: 0300 00e2 c020 c2e3 0003 82e1 0000 81e5  ..... ..........
-000036a0: 1f04 a0e3 3000 80e5 ff50 bde8 04f0 5ee2  ....0....P....^.
-000036b0: ff5f 2de9 0060 a0e3 0170 a0e3 0801 9fe5  ._-..`...p......
-000036c0: 0881 9fe5 f850 9fe5 0010 90e5 ec2f 98e5  .....P......./..
-000036d0: 0400 95e5 0100 80e2 0100 50e1 0400 85e5  ..........P.....
-000036e0: 0460 8525 0400 95e5 1700 12e1 f7ff ff0a  .`.%............
-000036f0: 0400 95e5 8043 88e0 3490 94e5 39a0 d4e5  .....C..4...9...
-00003700: 0100 a0e3 3e04 00eb 0420 95e5 ec1f 98e5  ....>.... ......
-00003710: 1712 d1e1 ec1f 88e5 b410 9f05 e224 a003  .............$..
-00003720: 0410 9105 1711 a001 0111 8102 7b15 8102  ............{...
-00003730: 0c10 8205 0110 a0e3 3a04 00eb 0100 5ae3  ........:.....Z.
-00003740: 3960 c4e5 1000 001a 2c07 00fa 0040 b0e1  9`......,....@..
-00003750: 0600 000a 0910 a0e1 0400 a0e1 5c04 00eb  ............\...
-00003760: 0010 a0e3 0400 a0e1 0f01 00fa 0300 00ea  ................
-00003770: 4b2f a0e3 3c10 8fe2 0000 a0e3 f507 00fa  K/..<...........
-00003780: 0900 a0e1 5807 00fa 0300 00ea 4420 9fe5  ....X.......D ..
-00003790: 2010 8fe2 0000 a0e3 ee07 00fa 1f04 a0e3   ...............
-000037a0: 3000 80e5 ff5f bde8 04f0 5ee2 7407 4000  0...._....^.t.@.
-000037b0: 107f 00e5 2531 0000 7363 616d 702d 6973  ....%1..scamp-is
-000037c0: 722e 6300 d000 4000 fd31 0000 e400 4000  r.c...@..1....@.
-000037d0: 0070 00e5 3c0b 4000 3301 0000 0020 2121  .p..<.@.3.... !!
-000037e0: 0906 10b5 8862 184b 0122 1821 1020 01f0  .....b.K.".!. ..
-000037f0: c9fe 0122 154b 1a21 1000 01f0 c3fe 144b  ...".K.!.......K
-00003800: 0122 1921 0220 01f0 bdfe 124b 0022 0b21  .".!. .....K.".!
-00003810: 0320 01f0 b7fe 104b 0122 0521 0420 01f0  . .....K.".!. ..
-00003820: b1fe 0e4b 0122 1421 0520 01f0 abfe 0c4b  ...K.".!. .....K
-00003830: 0122 0421 0620 01f0 a5fe 0a4b 0122 1221  .".!. .....K.".!
-00003840: 0720 01f0 9ffe 10bd e824 0000 0c25 0000  . .......$...%..
-00003850: 6425 0000 7c24 0000 fc47 0000 9001 0000  d%..|$...G......
-00003860: bc25 0000 b026 0000 4179 ff29 05d0 0288  .%...&..Ay.)....
-00003870: 521e 1204 120c 0280 01d0 0020 7047 0029  R.......... pG.)
-00003880: 07d0 491e 0906 090e 4171 02d1 ff21 4171  ..I.....Aq...!Aq
-00003890: 0ee0 4188 0180 8279 002a 06d0 521e 1206  ..A....y.*..R...
-000038a0: 120e 8271 01d1 0122 0271 0279 5143 4180  ...q...".q.yQCA.
-000038b0: 0120 7047 ff48 0021 0b00 c289 1204 08d5  . pG.H.!........
-000038c0: 8289 002a 05d0 521e 1204 120c 8281 00d1  ...*..R.........
-000038d0: c381 2030 491c 1029 efd3 7047 f549 0820  .. 0I..)..pG.I. 
-000038e0: 4201 5218 d289 002a 03d0 401c 0f28 f7d9  B.R....*..@..(..
-000038f0: ff20 7047 ffb5 81b0 8446 1d00 1700 fff7  . pG.....F......
-00003900: edff 0600 ff28 17d0 ea49 7001 4418 0320  .....(...Ip.D.. 
-00003910: 8003 2818 e081 0020 6781 a082 2100 6046  ..(.... g...!.`F
-00003920: fdf7 6efd 0298 211d fdf7 63fd 002d 02d0  ..n...!...c..-..
-00003930: 681e 0125 8540 a581 3000 05b0 f0bd de49  h..%.@..0......I
-00003940: 0120 0870 7047 0170 7047 827a 8189 c37a  . .ppG.ppG.z...z
-00003950: 8372 c272 c289 8281 c181 7047 70b5 0400  .r.r......pGp...
-00003960: 007a 0d00 0106 0fd5 4006 400e 2072 2000  .z......@.@. r .
-00003970: fff7 ebff 002d 02d0 0c20 2582 a080 0021  .....-... %....!
-00003980: 2000 00f0 13f9 70bd 2000 01f0 29fd 70bd   .....p. ...).p.
-00003990: f8b5 0f00 c949 0600 c001 4418 01f0 b8fd  .....I....D.....
-000039a0: 0500 01d1 8a20 f8bd 3900 2800 00f0 92ef  ..... ..9.(.....
-000039b0: 0120 2563 2034 2076 bf49 3439 895d 8840  . %c 4 v.I49.].@
-000039c0: bf49 4018 7121 4906 8860 0020 0090 bd48  .I@.q!I..`. ...H
-000039d0: 0222 6946 00f0 eeff 0600 07d1 ba4a bba1  ."iF.........J..
-000039e0: 01f0 bafe 2800 01f0 81fd dbe7 7d21 7769  ....(.......}!wi
-000039f0: c900 3000 01f0 3cff 207e 0028 03d0 6b46  ..0...<. ~.(..kF
-00003a00: 1878 0028 f8d0 6b46 1878 0028 04d0 2800  .x.(..kF.x.(..(.
-00003a10: 01f0 6cfd 8620 f8bd 3900 3000 01f0 f6fe  ..l.. ..9.0.....
-00003a20: 8020 f8bd a34a f0b5 4001 8418 e089 8fb0  . ...J..@.......
-00003a30: 0204 68d5 06aa 0232 0bab 0233 0293 8d88  ..h....2...3....
-00003a40: c305 04d5 0f00 1037 083d 0026 02e0 0f00  .......7.=.&....
-00003a50: 0837 0226 8005 01d5 a08a 02e0 9648 2038  .7.&.........H 8
-00003a60: 808a 6b46 0102 000a 0143 d985 ab19 0e93  ..kF.....C......
-00003a70: 1c33 1121 2000 fdf7 d4fc 0e9b 0833 1904  .3.! ........3..
-00003a80: 1802 090e 0843 6b46 5886 6089 0102 000a  .....CkFX.`.....
-00003a90: 0143 0020 1986 0200 9886 09a8 0821 0230  .C. .........!.0
-00003aa0: fdf7 3eee 0e9b 3100 1a18 0298 1932 0831  ..>...1......2.1
-00003ab0: fdf7 36ee 0200 2900 3800 fdf7 32ee c043  ..6...).8...2..C
-00003ac0: 0102 0004 000e 0143 6b46 9986 03a9 201d  .......CkF.... .
-00003ad0: 0191 fdf7 8efc 0199 7748 891d 1e38 fdf7  ........wH...8..
-00003ae0: 88fc 0820 6b46 1883 3200 2b00 2a32 3900  ... kF..2.+.*29.
-00003af0: 03a8 fdf7 dffc 0520 00f0 42fe e089 4004  ....... ..B...@.
-00003b00: 03d5 0020 e081 0fb0 f0bd 2069 401c 2061  ... ...... i@. a
-00003b10: f9e7 70b5 0400 007a 4206 02d5 4022 9043  ..p....zB...@".C
-00003b20: 2072 a589 e289 6c4b 9542 15d0 1a69 9542   r....lK.B...i.B
-00003b30: 12d0 8006 10d4 5869 0028 04d0 2800 01f0  ......Xi.(..(...
-00003b40: c9f9 0628 01d1 8721 2ce0 2100 2800 fdf7  ...(...!,.!.(...
-00003b50: f9ff 17e0 0100 25e0 a27a ff2a 04d1 607a  ......%..z.*..`z
-00003b60: 2100 fff7 5fff 0fe0 db68 d006 c00e 9842  !..._....h.....B
-00003b70: 01d3 8821 16e0 594b 1b68 8342 08d0 2100  ...!..YK.h.B..!.
-00003b80: fff7 06ff 8028 e5d1 2000 01f0 29fc 70bd  .....(.. ...).p.
-00003b90: 5009 06d1 2000 fff7 8dfb 0c30 0021 a080  P... ......0.!..
-00003ba0: 00e0 8521 2000 fff7 d9fe 70bd 0a00 0100  ...! .....p.....
-00003bb0: 4b48 0023 10b5 00f0 5fff 10bd f3b5 85b0  KH.#...._.......
-00003bc0: 0598 3d49 0700 0e37 1839 1e30 fdf7 1dfc  ..=I...7.9.0....
-00003bd0: 0028 6ed0 3878 0599 0007 800e 0e18 0e36  .(n.8x.........6
-00003be0: 7088 0106 090c 000a 0143 3088 0206 120c  p........C0.....
-00003bf0: 000a 0243 0392 b088 0206 150c 000a 0543  ...C...........C
-00003c00: 2d48 2038 808a 8842 40d1 ff20 0a3d 1930  -H 8...B@.. .=.0
-00003c10: 8542 6cdc 01f0 f4fb 0400 02d1 ff22 4d32  .Bl.........."M2
-00003c20: 6ee0 3100 2000 2a00 0a31 0830 00f0 5aee  n.1. .*..1.0..Z.
-00003c30: 2948 a580 0069 e081 3800 0c30 267a 657a  )H...i..8..0&zez
-00003c40: 0700 01a9 fdf7 dcfb ff2d 0bd1 3006 09d5  .........-..0...
-00003c50: 2148 0599 8368 039a 891d 3800 fff7 4afe  !H...h....8...J.
-00003c60: 0540 6572 1f48 0061 3006 07d5 102d 08d2  .@er.H.a0....-..
-00003c70: 1048 6901 0818 c089 0028 02d0 0199 2000  .Hi......(.... .
-00003c80: 70e0 2000 01f0 acfb 07b0 f0bd 083d ff20  p. ..........=. 
-00003c90: 1130 8542 0295 2adc 0024 064a 6001 8018  .0.B..*..$.J`...
-00003ca0: c289 002a 02d0 808a 8842 1ed0 641c 082c  ...*.....B..d..,
-00003cb0: 1ae0 1ce0 0c09 4000 7407 4000 0070 00e5  ......@.t.@..p..
-00003cc0: 0000 c05e 4729 0000 4a02 0000 7363 616d  ...^G)..J...scam
-00003cd0: 702d 332e 6300 0000 d800 4000 3c0b 4000  p-3.c.....@.<.@.
-00003ce0: 132b 0000 00c0 00e4 d7d3 082c 02d1 f748  .+.........,...H
-00003cf0: 0061 c9e7 01f0 84fb 0500 06d1 ff22 8532  .a...........".2
-00003d00: f349 0020 01f0 28fd f1e7 f24a 6001 8018  .I. ..(....J`...
-00003d10: 0399 0490 4181 3800 0499 0c30 fdf7 70fb  ....A.8....0..p.
-00003d20: 0498 011d 0598 801d fdf7 63fb 3100 2800  ..........c.1.(.
-00003d30: 029a 0831 1030 00f0 36ec e448 0061 0720  ...1.0..6..H.a. 
-00003d40: 2872 e548 6c72 0069 e881 ff20 e872 0298  (r.Hlr.i... .r..
-00003d50: 0021 0830 a880 0498 c08a a881 0498 007e  .!.0...........~
-00003d60: a872 2800 fff7 22ff 8ee7 10b5 d74c 6068  .r(..."......L`h
-00003d70: 4006 800e 02d1 1020 2062 10bd e06a d749  @......  b...j.I
-00003d80: 8006 000e 4018 0068 4105 606a 490d d44a  ....@..hA.`jI..J
-00003d90: 0005 000d 8018 027b 437b 1202 d218 0123  .......{C{.....#
-00003da0: db02 9a42 0ad1 c27d 112a 02d1 fff7 06ff  ...B...}.*......
-00003db0: dde7 012a 09d1 fdf7 2efc d8e7 c94b 9a42  ...*.........K.B
-00003dc0: 03d1 1022 fdf7 defb d1e7 2461 cfe7 c64a  ..."......$a...J
-00003dd0: c101 f8b5 8c18 0221 2500 2035 2976 c349  .......!%. 5)v.I
-00003de0: 095c 0120 8840 c249 4018 7121 4906 8860  .\. .@.I@.q!I..`
-00003df0: 0020 0090 bf48 0222 6946 00f0 dbfd 0600  . ...H."iF......
-00003e00: 04d1 bd4a b249 01f0 a7fc 18e0 7d21 7769  ...J.I......}!wi
-00003e10: c900 3000 01f0 2cfd 287e 0028 03d0 6b46  ..0...,.(~.(..kF
-00003e20: 1878 0028 f8d0 6b46 1878 0028 01d0 0020  .x.(..kF.x.(... 
-00003e30: f8bd 3900 3000 01f0 e9fc 206b a062 0120  ..9.0..... k.b. 
-00003e40: f8bd f8b5 0021 ff25 ac4b ca18 491c 1429  .....!.%.K..I..)
-00003e50: 1575 fad3 aa4a 0021 c418 a84e 1160 2175  .u...J.!...N.`!u
-00003e60: 2036 a149 3072 d161 0121 0022 7127 7f06   6.I0r.a.!."q'..
-00003e70: 8242 0ad0 3b69 0124 9440 2342 05d0 9f4b  .B..;i.$.@#B...K
-00003e80: d318 1975 8b19 491c 1a72 521c 122a efd3  ...u..I..rR..*..
-00003e90: 9148 c160 3177 02e0 8819 491c 0572 1429  .H.`1w....I..r.)
-00003ea0: fad3 3969 9748 8843 9149 4018 7860 9349  ..9i.H.C.I@.x`.I
-00003eb0: 8e48 1422 2831 00f0 16ed f8bd f0b5 924e  .H."(1.........N
-00003ec0: 0168 0660 8c46 0021 0127 3a00 8a40 491c  .h.`.F.!.':..@I.
-00003ed0: 9200 8358 8150 0468 8558 8350 8d42 01d1  ...X.P.h.X.P.B..
-00003ee0: b442 f2d0 6246 0260 0129 01d1 0020 f0bd  .B..bF.`.)... ..
-00003ef0: 491c 3800 8840 f0bd 8048 f8b5 2022 a038  I.8..@...H.. ".8
-00003f00: 8249 00f0 f0ec 7d49 7848 2022 6031 1430  .I....}IxH "`1.0
-00003f10: 00f0 e8ec 7e48 4022 0021 00f0 0eed 774d  ....~H@".!....wM
-00003f20: 803d a87a 0028 07d1 7048 1430 0088 0104  .=.z.(..pH.0....
-00003f30: 02d5 0006 000f a872 704e 704c 7548 4036  .......rpNpLuH@6
-00003f40: 403c 7060 a168 684f 8900 4018 3900 01f0  @<p`.hhO..@.9...
-00003f50: c7f8 0922 a060 1202 0021 3800 00f0 ecec  ...".`...!8.....
-00003f60: 6149 0720 2031 f760 8873 e869 5e49 4031  aI.  1.`.s.i^I@1
-00003f70: 4860 5d48 6849 4830 00f0 9eec 6178 ff20  H`]HhIH0....ax. 
-00003f80: 2530 4143 0022 a068 1300 01f0 21fb b062  %0AC.".h....!..b
-00003f90: ff22 a062 6178 2532 00f0 e8ff 4e48 e96a  .".bax%2....NH.j
-00003fa0: 3c30 00f0 7afa 4c48 a96b 3430 00f0 75fa  <0..z.LH.k40..u.
-00003fb0: 4948 6168 2c30 00f0 70fa 00f0 4aec 4107  IHah,0..p...J.A.
-00003fc0: 4548 490f 3430 0288 8918 0180 a078 0028  EHI.40.......x.(
-00003fd0: 06d1 4a48 2030 407f 0028 01d1 0120 2070  ..JH 0@..(...  p
-00003fe0: f8bd 4648 f8b5 6038 c088 00f0 9bfd 0327  ..FH..`8.......'
-00003ff0: 7f07 3800 fff7 62ff 404d 0100 403d 6e69  ..8...b.@M..@=ni
-00004000: 6f61 a869 4822 5043 3c4c 3818 4034 2060  oa.iH"PC<L8.@4 `
-00004010: ea68 891b 9200 cf19 8018 3900 01f0 60f8  .h........9...`.
-00004020: e860 0125 ad04 b108 7819 8900 0918 491b  .`.%....x.....I.
-00004030: a760 01f0 55f8 0022 2900 1300 2061 01f0  .`..U..")... a..
-00004040: c7fa 3649 2a00 a061 00f0 76ec 0022 3449  ..6I*..a..v.."4I
-00004050: 2069 1300 01f0 bcfa 0022 6061 2069 2900   i......."`a i).
-00004060: 1300 01f0 b5fa 2a00 0021 e061 00f0 64ec  ......*..!.a..d.
-00004070: 0022 ed11 2069 2900 1300 01f0 a9fa 2a00  .".. i).......*.
-00004080: 0021 6062 00f0 58ec f8bd 1c48 0022 4030  .!`b..X....H."@0
-00004090: 0121 10b5 0069 8902 1300 01f0 99fa 174c  .!...i.........L
-000040a0: 803c e16b 0029 0dd1 a522 cb07 02d0 8b00  .<.k.)..."......
-000040b0: c358 02e0 8b00 c358 db43 5a40 491c ff29  .X.....X.CZ@I..)
-000040c0: f3d9 e263 e06b 00f0 f1fb 10bd 00c0 00e4  ...c.k..........
-000040d0: cc2c 0000 0c09 4000 d800 4000 0080 00e4  .,....@...@.....
-000040e0: 0040 00e4 0608 0000 0070 00e5 4007 4000  .@.......p..@.@.
-000040f0: 0000 c05e 4729 0000 1e02 0000 807f 00e5  ...^G)..........
-00004100: 3c0b 4000 ffff 0300 aa55 00ff 504d 0000  <.@......U..PM..
-00004110: c07f 00f5 0001 00e5 744d 0000 ffff 0080  ........tM......
-00004120: 1040 0000 ea48 10b5 0088 c007 06d0 0120  .@...H......... 
-00004130: fdf7 84f8 e749 4007 c00f c872 10bd f1b5  .....I@....r....
-00004140: 0027 e54c e549 6068 e54d c201 5118 2031  .'.L.I`h.M..Q. 1
-00004150: 897b 0126 0429 04d3 fff7 39fe 0028 6068  .{.&.)....9..(`h
-00004160: 08d0 2f54 6068 401c 6060 e168 8842 00d3  ../T`h@.``.h.B..
-00004170: 6660 f8bd 295c 491c 0906 090e 2954 009a  f`..)\I.....)T..
-00004180: 9142 efd1 d249 1439 095c 3000 8840 0021  .B...I.9.\0..@.!
-00004190: fdf7 f4fa 6068 c101 d048 0818 0321 2030  ....`h...H...! 0
-000041a0: 8173 dfe7 f8b5 4024 0127 ca48 0088 0506  .s....@$.'.H....
-000041b0: 060a 3002 ff30 0130 2d0e 0090 4019 401c  ..0..0.0-...@.@.
-000041c0: 00f0 88fe 0628 00d0 4224 002d 05d1 0098  .....(..B$.-....
-000041d0: 00f0 80fe 0628 00d0 3c43 002e 06d1 681c  .....(..<C....h.
-000041e0: 00f0 78fe 0628 01d0 0420 0443 0022 bd49  ..x..(... .C.".I
-000041f0: 2300 d243 0020 00f0 2ffe f8bd f8b5 b64c  #..C. ../......L
-00004200: b44e e069 4036 401c e061 3078 b14d 0028  .N.i@6@..a0x.M.(
-00004210: 1cd0 2000 3c30 fff7 27fb 0028 16d0 ad48  .. .<0..'..(...H
-00004220: 0721 6030 c079 0902 c007 01d1 3f21 0902  .!`0.y......?!..
-00004230: 6888 2a88 0004 8018 fef7 fefd 3f22 1202  h.*.........?"..
-00004240: 0121 8907 1002 0123 fef7 f2f8 fff7 32fb  .!.....#......2.
-00004250: f078 0028 01d0 fff7 72ff 9e4f 0026 2037  .x.(....r..O.& 7
-00004260: f87a 0028 0cd0 9c4a 2432 1188 491c 0904  .z.(...J$2..I...
-00004270: 090c 8142 1180 03d3 0120 1680 01f0 86f8  ...B..... ......
-00004280: 9548 2c30 fff7 f0fa 0028 03d0 b97a bf20  .H,0.....(...z. 
-00004290: fef7 6af8 206a 0028 0dd1 e069 3228 0ad9  ..j. j.(...i2(..
-000042a0: 6888 ff38 0238 00f0 15fe 0628 03d0 0120  h..8.8.....(... 
-000042b0: 2062 fff7 77ff 6069 0028 1bd0 8648 3430   b..w.`i.(...H40
-000042c0: fff7 d2fa 0028 15d0 2078 874a 2169 1268  .....(.. x.J!i.h
-000042d0: 4008 0006 8900 5050 2069 844b 0104 2078  @.....PP i.K.. x
-000042e0: 3f22 c018 491c 1202 0023 fef7 a1f8 2078  ?"..I....#.... x
-000042f0: 801c 2070 688b 0028 0cd0 a169 491c 8142  .. ph..(...iI..B
-00004300: a161 07d3 3f22 a661 7948 296a 1202 0023  .a..?".ayH)j...#
-00004310: fef7 8ef8 f8bd feb5 0a21 7648 764c 0186  .........!vHvL..
-00004320: 0020 2062 0220 00f0 2bfa 6a48 2030 8188  .  b. ..+.jH 0..
-00004330: c088 4d00 4600 2900 6846 00f0 2cea 2800  ..M.F.).hF..,.(.
-00004340: 00f0 b9f8 6d4f 0099 c019 4018 2061 3100  ....mO....@. a1.
-00004350: 6846 00f0 20ea 3000 00f0 adf8 0099 c019  hF.. .0.........
-00004360: 4018 6061 5020 00f0 0bfa 5a48 ea03 807b  @.`aP ....ZH...{
-00004370: 604b 0109 491e 401e 8907 8007 090a 400b  `K..I.@.......@.
-00004380: 0818 5f49 120c 4018 1a86 2062 febd 70b5  .._I..@... b..p.
-00004390: 4f4d 2888 c007 2dd0 2c00 a81c fdf7 12f8  OM(...-.,.......
-000043a0: 4c48 2900 0422 0831 f030 00f0 9cea 2088  LH)..".1.0.... .
-000043b0: 4007 01d5 fcf7 08ff 2888 0007 09d5 ff21  @.......(......!
-000043c0: e231 0420 fcf7 26ff 0921 4902 0020 fcf7  .1. ..&..!I.. ..
-000043d0: 21ff 404c 0be0 0120 fcf7 30ff 4007 c00f  !.@L... ..0.@...
-000043e0: e072 e07a 0028 05d1 0120 00f0 4ffb 2888  .r.z.(... ..O.(.
-000043f0: 8007 f0d4 70bd 1021 4020 0176 0021 8076  ....p..!@ .v.!.v
-00004400: 0177 417f 4908 4900 4177 7047 70b5 a020  .wA.I.I.AwpGp.. 
-00004410: 384c 3d49 2086 3b48 0860 0020 e321 0906  8L=I .;H.`. .!..
-00004420: 8860 7120 4006 816b 0125 2943 8163 6068  .`q @..k.%)C.c`h
-00004430: fff7 07fd fff7 60fd 00f0 88ff fff7 6bff  ......`.......k.
-00004440: fff7 cffd fff7 21fe 6068 00f0 87fc 214e  ......!.`h....!N
-00004450: 4036 b078 0028 03d0 1e48 807a fef7 c2ff  @6.x.(...H.z....
-00004460: fdf7 03fa 208e 7d21 c900 4843 e222 2121  .... .}!..HC."!!
-00004470: 0906 8a60 0860 1648 2030 0570 fef7 06f8  ...`.`.H 0.p....
-00004480: fff7 acf9 b078 0028 01d0 fff7 80ff 0120  .....x.(....... 
-00004490: 00f0 fcfa 00f0 1aea f9e7 0a0e 0280 0a02  ................
-000044a0: 120e 4280 0a0a 4271 0a06 120f 0907 090f  ..B...Bq........
-000044b0: 8271 0171 7047 0021 3228 00d3 0121 6428  .q.qpG.!2(...!d(
-000044c0: 00d3 0221 c828 00d3 0321 0804 7047 0000  ...!.(...!..pG..
-000044d0: 5407 4000 007f 00e5 d800 4000 0070 00e5  T.@.......@..p..
-000044e0: f808 4000 5555 ffff 2c00 4000 0000 3e08  ..@.UU..,.@...>.
-000044f0: 0000 3e02 3c0b 4000 4000 00e2 0001 0400  ..>.<.@.@.......
-00004500: a588 1080 51e5 cc1a 000c 00e3 f041 2de9  ....Q........A-.
-00004510: 0150 a0e1 0070 a0e1 8040 9fe5 0260 a0e1  .P...p...@...`..
-00004520: b300 00eb 0210 d4e5 2000 51e3 0200 003a  ........ .Q....:
-00004530: ad00 00eb 0000 a0e3 f081 bde8 0210 d4e5  ................
-00004540: 0000 51e3 021b a003 1f24 a003 1010 8205  ..Q......$......
-00004550: 0210 d4e5 0110 81e2 0210 c4e5 0210 d4e5  ................
-00004560: 0320 d4e5 0200 51e1 0210 d485 0310 c485  . ....Q.........
-00004570: 0030 d4e5 8310 83e0 0111 84e0 0470 a1e5  .0...........p..
-00004580: 6000 81e9 0010 d4e5 0110 81e2 1f10 01e2  `...............
-00004590: 0010 c4e5 9400 00eb 0100 a0e3 f081 bde8  ................
-000045a0: 7407 4000 0300 52e3 2a00 009a 03c0 10e2  t.@...R.*.......
-000045b0: 0800 000a 0130 d1e4 0200 5ce3 0c20 82e0  .....0....\.. ..
-000045c0: 01c0 d194 0130 c0e4 0130 d134 01c0 c094  .....0...0.4....
-000045d0: 0420 42e2 0130 c034 0330 11e2 2500 000a  . B..0.4.0..%...
-000045e0: 0420 52e2 1b00 003a 03c0 31e7 0200 53e3  . R....:..1...S.
-000045f0: 0800 000a 0f00 008a 2c34 a0e1 04c0 b1e5  ........,4......
-00004600: 0420 52e2 0c3c 83e1 0430 80e4 f9ff ff2a  . R..<...0.....*
-00004610: 0110 81e2 0f00 00ea 2c38 a0e1 04c0 b1e5  ........,8......
-00004620: 0420 52e2 0c38 83e1 0430 80e4 f9ff ff2a  . R..8...0.....*
-00004630: 0210 81e2 0700 00ea 2c3c a0e1 04c0 b1e5  ........,<......
-00004640: 0420 52e2 0c34 83e1 0430 80e4 f9ff ff2a  . R..4...0.....*
-00004650: 0310 81e2 0000 a0e1 822f b0e1 0130 d124  ........./...0.$
-00004660: 01c0 d124 0120 d144 0130 c024 01c0 c024  ...$. .D.0.$...$
-00004670: 0120 c044 1eff 2fe1 1040 2de9 2020 52e2  . .D../..@-.  R.
-00004680: 0500 003a 1850 b1e8 2020 52e2 1850 a0e8  ...:.P..  R..P..
-00004690: 1850 b1e8 1850 a0e8 f9ff ff2a 02ce b0e1  .P...P.....*....
-000046a0: 1850 b128 1850 a028 1800 b148 1800 a048  .P.(.P.(...H...H
-000046b0: 1040 bde8 02cf b0e1 0430 9124 0430 8024  .@.......0.$.0.$
-000046c0: 1eff 2f01 822f b0e1 b230 d120 0120 d144  ../../...0. . .D
-000046d0: b230 c020 0120 c044 1eff 2fe1 04f0 1fe5  .0. . .D../.....
-000046e0: 9d09 0000 04f0 1fe5 7712 0000 04f0 1fe5  ........w.......
-000046f0: b710 0000 f2b5 0549 05a6 4027 3cce 3cc1  .......I..@'<.<.
-00004700: 103f fbd1 041c 3f39 0847 0000 c07f 0000  .?....?9.G......
-00004710: 0fcc 0128 08d0 0228 04d0 0328 0bd0 0428  ...(...(...(...(
-00004720: 11d0 f2bd 1219 103a e1ca e1c1 e1ca e1c1  .......:........
-00004730: 203b f9d8 ece7 1d1c 1e1c 1f1c e8c1 e8c1   ;..............
-00004740: 203a fbd8 e4e7 0098 8847 e1e7 0100 90e0   :.......G......
-00004750: 0100 8022 0008 90e0 0108 8022 ff0c c0e3  ..."......."....
-00004760: 0004 90e0 0104 8022 ff08 c0e3 0002 90e0  ......."........
-00004770: 0102 8022 0f02 00e2 0f02 20e2 1eff 2fe1  ..."...... .../.
-00004780: 0349 0988 4143 8808 0138 fdd2 7047 0000  .I..AC...8..pG..
-00004790: 6c0b 4000 0a20 41e2 2111 41e0 2112 81e0  l.@.. A.!.A.!...
-000047a0: 2114 81e0 2118 81e0 a111 a0e1 0131 81e0  !...!........1..
-000047b0: 8320 52e0 0110 8152 0a20 8242 0600 80e8  . R....R. .B....
-000047c0: 1eff 2fe1 0030 0fe1 01f0 21e1 00d0 a0e1  ../..0....!.....
-000047d0: 03f0 2fe1 0201 40e0 1eff 2fe1 0000 0fe1  ../...@.../.....
-000047e0: c010 80e3 01f0 21e1 1eff 2fe1 00f0 2fe1  ......!.../.../.
-000047f0: 1eff 2fe1 0000 0fe1 8010 80e3 01f0 21e1  ../...........!.
-00004800: 1eff 2fe1 e2c4 a0e3 00c1 8ce0 0000 0fe1  ../.............
-00004810: c010 80e3 01f0 21e1 0011 9ce5 0201 11e3  ......!.........
-00004820: fcff ff1a 1eff 2fe1 e2c4 a0e3 0111 8ce0  ....../.........
-00004830: 8011 91e5 00f0 21e1 1eff 2fe1 0120 52e2  ......!.../.. R.
-00004840: 0130 d124 0130 c024 fbff ff2a 1eff 2fe1  .0.$.0.$...*../.
-00004850: 1c30 9fe5 0300 93e8 a100 11e1 6020 b0e1  .0..........` ..
-00004860: 0110 a1e0 0026 22e0 220a 22e0 0300 83e8  .....&".".".....
-00004870: 1eff 2fe1 440b 4000 0f50 2de9 0400 4ee2  ../.D.@..P-...N.
-00004880: 00c0 4fe1 1ff0 21e3 0050 2de9 5602 00fa  ..O...!..P-.V...
-00004890: 0050 bde8 92f0 21e3 0cf0 6fe1 2f04 a0e3  .P....!...o./...
-000048a0: 3000 80e5 0f50 bde8 04f0 5ee2 014a 0021  0....P....^..J.!
-000048b0: 03c2 7047 440b 4000 0120 d1e4 0000 52e3  ..pGD.@.. ....R.
-000048c0: 0120 c0e4 fbff ff1a 1eff 2fe1 900f 07ee  . ......../.....
-000048d0: 1eff 2fe1 0400 80e2 0410 81e2 b020 d1e1  ../.......... ..
-000048e0: 0420 82e2 0300 12e3 0320 c213 0420 8212  . ....... ... ..
-000048f0: 1040 2de9 2020 52e2 0500 003a 1850 b1e8  .@-.  R....:.P..
-00004900: 1850 a0e8 1850 b1e8 1850 a0e8 2020 52e2  .P...P...P..  R.
-00004910: f9ff ff2a 02ce b0e1 1850 b128 1850 a028  ...*.....P.(.P.(
-00004920: 1800 b148 1800 a048 02cf b0e1 0430 9124  ...H...H.....0.$
-00004930: 0430 8024 1080 bde8 0130 a0e1 1020 52e2  .0.$.....0... R.
-00004940: 0a00 a028 0a00 a028 fbff ff2a 822e b0e1  ...(...(...*....
-00004950: 0a00 a028 0200 a048 1eff 2fe1 01c0 5ee5  ...(...H../...^.
-00004960: 0c00 53e1 0330 de37 0c30 de27 83c0 8ee0  ..S..0.7.0.'....
-00004970: 1cff 2fe1 70b5 0600 1821 00f0 ebfa 0c4d  ../.p....!.....M
-00004980: 0400 0ed0 1822 3100 2000 00f0 effa 0600  ....."1. .......
-00004990: fff7 24ef 2968 3160 2c60 fff7 28ef 0120  ..$.)h1`,`..(.. 
-000049a0: 70bd 6869 0821 0843 6861 0020 70bd 0000  p.hi.!.Cha. p...
-000049b0: 780b 4000 f8b5 0500 0e00 1700 fff7 0eef  x.@.............
-000049c0: 134a 1468 002c 17d0 d168 491c 00d1 0121  .J.h.,...hI....!
-000049d0: 2368 1360 0023 2360 d160 e760 a660 6560  #h.`.##`.`.`.`e`
-000049e0: 2361 6161 1189 491c 0904 090c 1181 5389  #aaa..I.......S.
-000049f0: 9942 08d9 5181 06e0 1169 1023 491c 1161  .B..Q....i.#I..a
-00004a00: 5169 1943 5161 fff7 f2ee 2000 f8bd 0000  Qi.CQa.... .....
-00004a10: 780b 4000 70b5 0500 084c 03d0 0120 2076  x.@.p....L...  v
-00004a20: 0a20 02e0 0020 2076 0720 00f0 3dfb 226b  . ...  v. ..=."k
-00004a30: 002a 02d0 616b 2800 9047 70bd 780b 4000  .*..ak(..Gp.x.@.
-00004a40: 70b5 0500 0329 01d9 0020 70bd c800 0949  p....)... p....I
-00004a50: 4418 fff7 c4ee a16f 7834 0029 02d1 6560  D......ox4.)..e`
-00004a60: 2560 02e0 6168 0d60 6560 fff7 c0ee 0120  %`..ah.`e`..... 
-00004a70: 70bd 0000 780b 4000 10b5 1c00 fff7 9aff  p...x.@.........
-00004a80: 0028 02d0 2100 fff7 dbff 10bd f1b5 0025  .(..!..........%
-00004a90: 2f00 82b0 29e0 1748 e900 0e18 fff7 9eee  /...)..H........
-00004aa0: b46f b767 fff7 a2ee 0194 11e0 6268 2668  .o.g........bh&h
-00004ab0: e168 a068 9047 fff7 92ee 0e49 0a68 2260  .h.h.G.....I.h"`
-00004ac0: 0c60 6761 0a89 521e 0a81 fff7 90ee 3400  .`ga..R.......4.
-00004ad0: 002c ebd1 0198 0028 04d0 0298 0028 01d0  .,.....(.....(..
-00004ae0: 0025 02e0 6d1c 032d 03d8 0248 017e 0029  .%..m..-...H.~.)
-00004af0: d1d0 febd 780b 4000 0449 0222 0a76 1f23  ....x.@..I.".v.#
-00004b00: ca6c 1b06 5a61 8863 7047 0000 780b 4000  .l..Za.cpG..x.@.
-00004b10: ca08 9200 4907 8058 c90e c840 0007 000f  ....I..X...@....
-00004b20: 7047 0000 1c49 f8b5 4843 0721 030a 0320  pG...I..HC.!... 
-00004b30: 4907 4860 0420 4860 184d 0022 6a60 184c  I.H`. H`.M."j`.L
-00004b40: 1000 4600 8700 a65b 7f18 7e61 401c 0e28  ..F....[..~a@..(
-00004b50: f7d3 1448 c860 0b61 144b 1348 1860 0320  ...H.`.a.K.H.`. 
-00004b60: 8004 8860 8a60 5802 8860 8860 1048 8860  ...`.`X..`.`.H.`
-00004b70: 0520 4004 8860 4a60 aa60 d803 6860 6424  . @..`J`.`..h`d$
-00004b80: 03e0 0120 fff7 fcfd 641e 2868 4003 01d4  ... ....d.(h@...
-00004b90: 002c f6d1 2000 f8bd cd07 0000 0003 00e0  .,.. ...........
-00004ba0: 804d 0000 1280 0100 e060 0000 0002 00e0  .M.......`......
-00004bb0: 3300 0800 0149 0820 c872 7047 207f 00e5  3....I. .rpG ...
-00004bc0: f3b5 81b0 0600 00d1 febd 1d48 4569 0720  ...........HEi. 
-00004bd0: fff7 18ee 1a49 0023 2031 0c88 07e0 2701  .....I.# 1....'.
-00004be0: ea5b a119 9142 09d9 2300 7919 4c88 002c  .[...B..#.y.L..,
-00004bf0: f5d1 0721 fff7 18ee 2000 febd 9142 08d2  ...!.... ....B..
-00004c00: 0e01 aa53 2201 a952 7a19 5788 7619 7780  ...S"..Rz.W.v.w.
-00004c10: 5180 002b 06d0 2101 4919 1a01 4988 5219  Q..+..!.I...I.R.
-00004c20: 5180 05e0 2101 064a 4919 4988 2032 1180  Q...!..JI.I. 2..
-00004c30: 0299 0122 d203 1143 2201 5219 5180 d8e7  ..."...C".R.Q...
-00004c40: c07f 00e5 30b5 e124 0749 2406 e162 074b  ....0..$.I$..b.K
-00004c50: 0021 8a00 8558 9d50 491c 1029 f9d3 0248  .!...X.PI..)...H
-00004c60: c043 e062 30bd 0000 0000 ffff 0002 00e1  .C.b0...........
-00004c70: f3b5 83b0 0700 2749 401e 8842 47d2 2648  ......'I@..BG.&H
-00004c80: 4569 0720 fff7 beed 0190 2348 0499 2030  Ei. ......#H.. 0
-00004c90: 0488 3801 0026 0029 0290 0bd0 285a c11b  ..8..&.)....(Z..
-00004ca0: 3800 00f0 71f8 05e0 a742 05d3 2600 2001  8...q....B..&. .
-00004cb0: 4019 4488 002c f7d1 0298 3904 4019 090c  @.D..,....9.@...
-00004cc0: 002e 4480 03d0 3201 5219 5180 02e0 124a  ..D...2.R.Q....J
-00004cd0: 2032 1180 002c 0ad0 0299 695a a142 06d1   2...,....iZ.B..
-00004ce0: 2101 6b5a 029a 4919 ab52 4988 4180 002e  !.kZ..I..RI.A...
-00004cf0: 09d0 3101 6a5a ba42 05d1 029a aa5a 6a52  ..1.jZ.B.....ZjR
-00004d00: 4088 4919 4880 0198 0721 fff7 8eed 05b0  @.I.H....!......
-00004d10: f0bd 0000 ff03 0000 c07f 00e5 f3b5 81b0  ................
-00004d20: 0026 0700 0b48 4469 0120 c103 0f43 0ae0  .&...HDi. ...C..
-00004d30: 2919 4988 084a 1140 b942 03d1 0299 fff7  ).I..J.@.B......
-00004d40: 97ff 761c 605b 0501 615b 0029 f0d1 3000  ..v.`[..a[.)..0.
-00004d50: febd 0000 c07f 00e5 ffe0 0000 10b5 0400  ................
-00004d60: 00f0 cef8 0020 00f0 3bf8 0548 fff7 6aff  ..... ..;..H..j.
-00004d70: 0449 2002 0843 e121 0906 0860 10bd 0000  .I ..C.!...`....
-00004d80: 9c4d 0000 0100 4000 f0b5 4518 0121 8902  .M....@...E..!..
-00004d90: 8d42 01d9 0020 f0bd 0d49 0e4f 4c69 0026  .B... ...I.OLi.&
-00004da0: 12e0 0d49 ff23 8200 1b06 5118 0b60 0101  ...I.#....Q..`..
-00004db0: 0919 4b60 094b d318 1e60 0023 db43 d219  ..K`.K...`.#.C..
-00004dc0: ce60 1360 401c 8b60 8542 ead8 0120 f0bd  .`.`@..`.B... ..
-00004dd0: c07f 00e5 0080 00e1 0040 00e1 00c0 00e1  .........@......
-00004de0: 10b5 0124 a402 211a fff7 ceff 0848 084a  ...$..!......H.J
-00004df0: 4069 0121 2032 1180 0021 0482 2201 4182  @i.! 2...!..".A.
-00004e00: 8018 0180 4180 ff21 0906 4160 10bd 0000  ....A..!..A`....
-00004e10: c07f 00e5 ffb5 0400 0e00 00d1 6688 0120  ............f.. 
-00004e20: 8002 8642 09d8 1f06 0025 11e0 2088 0299  ...B.....%.. ...
-00004e30: 4018 0121 8902 8842 02d3 0020 04b0 f0bd  @..!...B... ....
-00004e40: 6168 e268 cb19 a168 00f0 06f8 1034 6d1c  ah.h...h.....4m.
-00004e50: b542 ebd3 0120 f1e7 ffb5 0600 0120 0f00  .B... ....... ..
-00004e60: 8002 8642 02d3 0020 04b0 f0bd 1448 3101  ...B... .....H1.
-00004e70: 4069 4418 180e 01d1 4020 007f 1d02 1149  @iD.....@ .....I
-00004e80: 2d0a 6560 0968 0902 0818 0121 c903 4018  -.e`.h.....!..@.
-00004e90: 6080 a809 00f0 30fd aa06 920e 8101 1143  `.....0........C
-00004ea0: 094a b000 8218 1160 0849 094a 4118 0f60  .J.....`.I.JA..`
-00004eb0: a760 0299 8018 0160 0120 e160 d4e7 0000  .`.....`. .`....
-00004ec0: c07f 00e5 3c0b 4000 0040 00e1 0080 00e1  ....<.@..@......
-00004ed0: 00c0 00e1 0122 c108 5203 9142 01d3 0620  ....."..R..B... 
-00004ee0: 7047 4007 400f 4200 8018 044a 8900 8918  pG@.@.B....J....
-00004ef0: 0968 c140 4807 400f 7047 0000 0000 01e1  .h.@H.@.pG......
-00004f00: 0649 074a 0020 0123 5b03 10b5 8400 a418  .I.J. .#[.......
-00004f10: 401c 9842 2160 f9d3 10bd 0000 b66d db00  @..B!`.......m..
-00004f20: 0000 01e1 0123 c208 5b03 9a42 10b5 0dd2  .....#..[..B....
-00004f30: 4007 400f 4300 c018 9300 054a 0724 9a18  @.@.C......J.$..
-00004f40: 8440 1368 8140 a343 1943 1160 10bd 0000  .@.h.@.C.C.`....
-00004f50: 0000 01e1 4143 0448 0022 10b5 8069 1300  ....AC.H."...i..
-00004f60: 00f0 36fb 10bd 0000 3c0b 4000 0300 491e  ..6.....<.@...I.
-00004f70: 02d0 8018 1860 f9e7 0021 1960 7047 1430  .....`...!.`pG.0
-00004f80: 10b5 07c8 fff7 d8ec 0020 10bd 70b5 0300  ......... ..p...
-00004f90: 8069 ff22 d969 0132 9042 01d8 0229 03d9  .i.".i.2.B...)..
-00004fa0: 8420 1882 0020 70bd 5c69 1433 0029 06d1  . ... p.\i.3.)..
-00004fb0: 02e0 625c 5a54 491c 8142 fad3 70bd 0129  ..b\ZTI..B..p..)
-00004fc0: 09d1 0021 4508 03e0 4a00 a65a 491c 9e52  ...!E...J..ZI..R
-00004fd0: 8d42 f9d8 70bd 0021 8508 03e0 8a00 a658  .B..p..!.......X
-00004fe0: 491c 9e50 8d42 f9d8 70bd 0000 0a49 10b5  I..P.B..p....I..
-00004ff0: 0988 0a04 0949 4b68 0968 1b02 d218 5118  .....IKh.h....Q.
-00005000: 4161 0749 8161 0749 0968 c161 2030 06a1  Aa.I.a.I.h.a 0..
-00005010: fff7 52ec 1b20 10bd 007f 00e5 3c0b 4000  ..R.. ......<.@.
-00005020: 0001 8500 704d 0000 5341 524b 2f53 7069  ....pM..SARK/Spi
-00005030: 4e4e 616b 6572 0000 30b5 ff23 8269 c169  NNaker..0..#.i.i
-00005040: 0133 9a42 01d8 0229 02d9 8421 0182 1fe0  .3.B...)...!....
-00005050: 4369 2030 0029 06d1 02e0 445c 5c54 491c  Ci 0.)....D\\TI.
-00005060: 9142 fad3 14e0 0129 09d1 0021 5408 03e0  .B.....)...!T...
-00005070: 4a00 855a 491c 9d52 8c42 f9d8 08e0 0021  J..ZI..R.B.....!
-00005080: 9408 03e0 8a00 8558 491c 9d50 8c42 f9d8  .......XI..P.B..
-00005090: 0020 30bd 0021 02e0 491c 421e 1040 0028  . 0..!..I.B..@.(
-000050a0: fad1 0800 7047 0000 0249 c969 2031 8873  ....pG...I.i 1.s
-000050b0: 7047 0000 3c0b 4000 0300 2de9 0202 a0e3  pG..<.@...-.....
-000050c0: 1400 90e5 1000 9fe5 3810 90e5 0110 81e2  ........8.......
-000050d0: 3810 80e5 0300 bde8 04f0 5ee2 3c0b 4000  8.........^.<.@.
-000050e0: 0200 0c32 0839 4260 c160 0260 0023 8160  ...2.9B`.`.`.#.`
-000050f0: 0b60 0361 4b60 7047 70b5 4025 2988 0400  .`.aK`pGp.@%)...
-00005100: 8900 401a 6a88 d221 fff7 5ceb aa88 d121  ..@.j..!..\....!
-00005110: fff7 58eb 0022 df21 fff7 54eb e888 8108  ..X..".!..T.....
-00005120: 8900 611a 2a4c 0020 2161 c06c 6061 fff7  ..a.*L. !a.l`a..
-00005130: d7ff a061 2806 4069 2649 000e 6060 4018  ...a(.@i&I..``@.
-00005140: 007d 2060 2348 ff26 6038 8088 2086 2248  .} `#H.&`8.. ."H
-00005150: 2536 a060 287e 3100 fff7 fcfe 2062 297e  %6.`(~1..... b)~
-00005160: 3200 fff7 03ff 2168 1229 1ed2 1b4a c801  2.....!h.)...J..
-00005170: 8018 184a e061 403a 9369 5269 4b43 9900  ...J.a@:.iRiKC..
-00005180: 8918 6163 7022 0021 fff7 d6eb e069 0522  ..acp".!.....i."
-00005190: 0100 2031 8a73 2a7f ca73 0e49 8039 c969  .. 1.s*..s.I.9.i
-000051a0: 4164 0f49 4830 fff7 88eb 00f0 cbf9 687e  Ad.IH0........h~
-000051b0: 0c4b 0122 1221 00f0 e5f9 0b4b 0122 0621  .K.".!.....K.".!
-000051c0: 1020 00f0 dff9 a87e fff7 d4fb 1f20 70bd  . .....~..... p.
-000051d0: 3c0b 4000 807f 00e5 adde adde 0070 00e5  <.@..........p..
-000051e0: 744d 0000 7838 0000 b840 0000 f8b5 0121  tM..x8...@.....!
-000051f0: 524f 7a68 9140 524a 8918 7122 5206 d160  ROzh.@RJ..q"R..`
-00005200: fb69 1c00 2034 217e 0029 18d0 1a6b 0229  .i.. 4!~.)...k.)
-00005210: 00d1 1863 0025 2576 1f26 3606 0329 20d1  ...c.%%v.&6..) .
-00005220: d31e fff7 9ceb 0b11 0c0c 0709 0d1c 1717  ................
-00005230: 1717 0c00 0120 00e0 0020 fff7 ebfb f8bd  ..... ... ......
-00005240: ff20 fff7 59fc f8bd 4020 417f 4908 4900  . ..Y...@ A.I.I.
-00005250: 4177 f8bd 3b48 c262 0120 4007 67e0 1020  Aw..;H.b. @.g.. 
-00005260: 65e0 0129 f5d1 0092 00f0 caf8 0400 60d0  e..)..........`.
-00005270: 0099 2000 fff7 2eeb 0098 00f0 37f9 b86a  .. .........7..j
-00005280: 401c b862 a77a 3806 400f 31d1 a088 1828  @..b.z8.@.1....(
-00005290: 01d2 8120 1be0 208a 8021 0028 2182 03d1  ... .. ..!.(!...
-000052a0: 2000 fff7 a3fe 14e0 0228 03d1 2000 fff7   ........(.. ...
-000052b0: 6dfe 0ee0 0328 03d1 2000 fff7 bdfe 08e0  m....(.. .......
-000052c0: 0528 03d1 2000 fff7 5afe 02e0 8320 2082  .(.. ...Z....  .
-000052d0: 2800 0c30 a080 a07a a189 e27a a272 e072  (..0...z...z.r.r
-000052e0: e089 a081 e181 0a21 2000 00f0 a3f8 13e0  .......! .......
-000052f0: 4020 c07e 0028 13d0 1348 8069 0028 0bd0  @ .~.(...H.i.(..
-00005300: fff7 6cea 0500 7a09 2100 0320 00f0 1efa  ..l...z.!.. ....
-00005310: 2800 fff7 6cea f8bd 2000 00f0 61f8 f8bd  (...l... ...a...
-00005320: 3069 c000 f8d5 0748 8462 0120 0007 b061  0i.....H.b. ...a
-00005330: f8bd 0098 00f0 daf8 f8bd 0000 3c0b 4000  ............<.@.
-00005340: 0000 c05e 780b 4000 0c0b 4000 f8b5 0021  ...^x.@...@....!
-00005350: 0c48 fff7 ddfb 0600 0024 0125 2f00 08e0  .H.......$.%/...
-00005360: 0848 2900 fff7 d4fb 0100 3800 8840 0443  .H).......8..@.C
-00005370: 6d1c b542 f4d9 0448 8460 4168 a143 4160  m..B...H.`Ah.CA`
-00005380: f8bd 0000 307f 00e5 4000 00e2 f8b5 0400  ....0...@.......
-00005390: 0021 1148 fff7 bcfb 0700 104e 0125 18e0  .!.H.......N.%..
-000053a0: 0d48 2900 fff7 b4fb 0100 0120 8840 e107  .H)........ .@..
-000053b0: 2200 0223 c90f 1a40 a408 002a 03d1 0029  "..#...@...*...)
-000053c0: 06d0 3168 0140 0029 01d0 f060 00e0 b060  ..1h.@.)...`...`
-000053d0: 6d1c bd42 e4d9 f8bd 307f 00e5 4000 00e2  m..B....0...@...
-000053e0: 70b5 0500 054c fff7 fae9 216a 2960 2562  p....L....!j)`%b
-000053f0: a18c 491e a184 fff7 fae9 70bd 3c0b 4000  ..I.......p.<.@.
-00005400: 70b5 0b4c fff7 eae9 256a 2034 002d 0ad0  p..L....%j 4.-..
-00005410: 2968 2160 a188 491c 0904 090c a180 e288  )h!`..I.........
-00005420: 9142 00d9 e180 fff7 e2e9 2800 70bd 0000  .B........(.p...
-00005430: 3c0b 4000 f8b5 0d00 0600 00f0 69f8 0400  <.@.........i...
-00005440: 01d1 0020 f8bd 3100 2000 fff7 44ea 1c4e  ... ..1. ...D..N
-00005450: 0127 f069 4463 2030 4776 3800 fff7 d2e9  .'.iDc 0Gv8.....
-00005460: 3268 1849 3b00 9340 c96a 164a 0b43 0029  2h.I;..@.j.J.C.)
-00005470: d362 08d1 1349 7122 2039 097a 8f40 1249  .b...Iq" 9.z.@.I
-00005480: 7918 5206 9160 0121 fff7 cee9 0d49 b039  y.R..`.!.....I.9
-00005490: 0a68 f069 2030 03e0 0b68 9b1a ab42 02d8  .h.i 0...h...B..
-000054a0: 437e 002b f8d1 407e 0028 03d0 2000 00f0  C~.+..@~.(.. ...
-000054b0: 1df8 c6e7 f06a 401c f062 0120 f8bd 0000  .....j@..b. ....
-000054c0: 3c0b 4000 c07f 00e5 0000 c05e 0248 0b21  <.@........^.H.!
-000054d0: c069 2030 8173 7047 3c0b 4000 0248 0621  .i 0.spG<.@..H.!
-000054e0: c069 2030 8173 7047 3c0b 4000 10b5 0400  .i 0.spG<.@.....
-000054f0: 0020 fff7 88e9 0549 0a68 2260 0c60 8a88  . .....I.h"`.`..
-00005500: 521e 8a80 0021 fff7 90e9 10bd 687f 00e5  R....!......h...
-00005510: 0020 10b5 fff7 76e9 0949 0c68 002c 0ad0  . ....v..I.h.,..
-00005520: 2268 0a60 8a88 521c 1204 120c 8a80 cb88  "h.`..R.........
-00005530: 9a42 00d9 ca80 0021 fff7 76e9 2000 10bd  .B.....!..v. ...
-00005540: 687f 00e5 0020 f0b5 c043 1f24 2406 6061  h.... ...C.$$.`a
-00005550: 0022 e260 2263 074b 074d 084f 1000 8100  .".`"c.K.M.O....
-00005560: ce18 3260 c919 0d60 401c 1028 f7d3 0448  ..2`...`@..(...H
-00005570: 6063 f0bd 0002 001f 0801 0000 0001 001f  `c..............
-00005580: a838 0000 70b5 0124 8c40 1f25 2d06 1028  .8..p..$.@.%-..(
-00005590: 03d1 0020 c363 ec60 08e0 064e 8000 8619  ... .c.`...N....
-000055a0: 3360 2023 1943 044b c018 0160 002a 00d0  3` #.C.K...`.*..
-000055b0: 2c61 70bd 0001 001f 0002 001f 10b5 4024  ,ap...........@$
-000055c0: 01e0 fff7 84e9 607f c007 fad1 10bd 0000  ......`.........
-000055d0: ffb5 81b0 1600 1d00 0029 30d0 ff2e 2ed8  .........)0.....
-000055e0: 280a aa07 01d4 4020 007f 0002 8719 002e  (.....@ ........
-000055f0: 05d0 2748 ba00 c069 8058 0028 1fd1 c91c  ..'H...i.X.(....
-00005600: 8808 8000 0830 0290 e807 03d0 0620 fff7  .....0....... ..
-00005610: fae8 8446 0198 0022 0468 08e0 0298 2168  ...F...".h....!h
-00005620: 2018 a042 05d9 8842 0cd9 2200 6468 002c   ..B...B..".dh.,
-00005630: f4d1 e807 03d0 0621 6046 fff7 f6e8 0020  .......!`F..... 
-00005640: 05b0 f0bd 0300 0833 8b42 04d2 0160 2060  .......3.B...` `
-00005650: 6168 4160 6060 002a 02d0 6068 5060 02e0  ahA```.*..`hP`..
-00005660: 0198 6168 0160 e807 03d0 0621 6046 fff7  ..ah.`.....!`F..
-00005670: dce8 0120 0004 381a 002e 6060 05d0 0449  ... ..8...``...I
-00005680: 2000 c969 0830 ba00 8850 2000 0830 d7e7   ..i.0...P ..0..
-00005690: c07f 00e5 f8b5 0500 0c00 1600 0029 02d1  .............)..
-000056a0: 1020 fbf7 44ed f007 03d0 0620 fff7 aae8  . ..D...... ....
-000056b0: 0090 083c 6268 2868 1204 0021 120c 1306  ...<bh(h...!....
-000056c0: 09d0 154f 0023 ff69 9200 bb50 03e0 8442  ...O.#.i...P...B
-000056d0: 03d3 0100 4068 0028 f9d1 0029 6060 01d0  ....@h.(...)``..
-000056e0: 4c60 00e0 2c60 0028 06d0 2268 8242 03d1  L`..,`.(.."h.B..
-000056f0: 0268 2260 4068 6060 0029 06d0 0868 a042  .h"`@h``.)...h.B
-00005700: 03d1 2068 0860 6068 4860 f007 03d0 0098  .. h.``hH`......
-00005710: 0621 fff7 8ae8 f8bd c07f 00e5 f7b5 0700  .!..............
-00005720: 0e00 4468 0025 0ce0 6068 0004 000e 8642  ..Dh.%..`h.....B
-00005730: 06d1 2100 029a 0831 3800 fff7 abff 6d1c  ..!....18.....m.
-00005740: 2468 2068 0028 efd1 2800 febd 7047 0000  $h h.(..(...pG..
-00005750: 01c0 8fe2 1cff 2fe1 10b5 0e4c e369 1a64  ....../....L.i.d
-00005760: d963 598f 0c4a 9142 01d0 491c 5987 2168  .cY..J.B..I.Y.!h
-00005770: 0029 02d0 094a 1021 d172 0228 06d0 0028  .)...J.!.r.(...(
-00005780: 07d1 0448 2030 807c 0028 02d0 0d20 fbf7  ...H 0.|.(... ..
-00005790: ceec 10bd 3c0b 4000 ffff 0000 207f 00e5  ....<.@..... ...
-000057a0: 2122 70b5 1206 d262 134d 0024 6868 2600  !"p....b.M.$hh&.
-000057b0: 04e0 0168 6960 0460 0400 0800 0028 14d0  ...hi`.`.....(..
-000057c0: 0169 0029 f5d0 1162 0661 0ee0 6268 002a  .i.)...b.a..bh.*
-000057d0: 02d0 e168 a068 9047 2068 2968 2160 2c60  ...h.h.G h)h!`,`
-000057e0: 6661 2989 491e 0400 2981 002c eed1 1f20  fa).I...)..,... 
-000057f0: 0006 0063 70bd 0000 780b 4000 0f50 2de9  ...cp...x.@..P-.
-00005800: e6ff fffa 0f50 bde8 04f0 5ee2 70b5 0400  .....P....^.p...
-00005810: 0d00 0028 02d1 1020 fbf7 88ec 6069 a842  ...(... ....`i.B
-00005820: 23d1 fef7 dcef 114b 0025 5a68 a242 01d1  #......K.%Zh.B..
-00005830: 6560 18e0 1168 14e0 a142 10d1 2168 1160  e`...h...B..!h.`
-00005840: 2168 0029 03d0 0a69 2669 9219 0a61 1968  !h.)...i&i...a.h
-00005850: 2160 1c60 6561 1989 491e 1981 03e0 0a00  !`.`ea..I.......
-00005860: 0968 0029 e8d1 fef7 c2ef 70bd 780b 4000  .h.)......p.x.@.
-00005870: f8b5 0400 1848 058e 4d43 fef7 b0ef 1749  .....H..MC.....I
-00005880: 2122 4b68 1206 002b 04d1 4c60 1562 e321  !"Kh...+..L`.b.!
-00005890: 9162 1ee0 576a bd42 05d2 1562 7a1b 1a61  .b..Wj.B...bz..a
-000058a0: 2360 4c60 15e0 0022 1600 1968 ef1b 09e0  #`L`..."...h....
-000058b0: 0d69 aa18 ba42 02d9 d21b 0a61 04e0 0b00  .i...B.....a....
-000058c0: 0968 ae19 0029 f3d1 b91b 2161 1968 2160  .h...)....!a.h!`
-000058d0: 1c60 fef7 8cef f8bd 3c0b 4000 780b 4000  .`......<.@.x.@.
-000058e0: 10b5 1c00 fff7 66f8 0028 03d0 2100 fff7  ......f..(..!...
-000058f0: bfff 0120 10bd 0000 0200 70b5 0020 084c  ... ......p.. .L
-00005900: 0100 0123 1d00 8d40 1542 04d0 0d19 2d7a  ...#...@.B....-z
-00005910: 1e00 ae40 3043 491c 1229 f3d3 70bd 0000  ...@0CI..)..p...
-00005920: a07f 00e5 ffff ffff ffff 0000 0000 0000  ................
-00005930: 0000 0000 ffff 0001 0100 0000 00ff ff00  ................
-00005940: 0101 0000 0000 8200 0000 0000 0000 0000  ................
-00005950: 0000 0000 9630 0777 2c61 0eee ba51 0999  .....0.w,a...Q..
-00005960: 19c4 6d07 8ff4 6a70 35a5 63e9 a395 649e  ..m...jp5.c...d.
-00005970: 3288 db0e a4b8 dc79 1ee9 d5e0 88d9 d297  2......y........
-00005980: 2b4c b609 bd7c b17e 072d b8e7 911d bf90  +L...|.~.-......
-00005990: 6410 b71d f220 b06a 4871 b9f3 de41 be84  d.... .jHq...A..
-000059a0: 7dd4 da1a ebe4 dd6d 51b5 d4f4 c785 d383  }......mQ.......
-000059b0: 5698 6c13 c0a8 6b64 7af9 62fd ecc9 658a  V.l...kdz.b...e.
-000059c0: 4f5c 0114 d96c 0663 633d 0ffa f50d 088d  O\...l.cc=......
-000059d0: c820 6e3b 5e10 694c e441 60d5 7271 67a2  . n;^.iL.A`.rqg.
-000059e0: d1e4 033c 47d4 044b fd85 0dd2 6bb5 0aa5  ...<G..K....k...
-000059f0: faa8 b535 6c98 b242 d6c9 bbdb 40f9 bcac  ...5l..B....@...
-00005a00: e36c d832 755c df45 cf0d d6dc 593d d1ab  .l.2u\.E....Y=..
-00005a10: ac30 d926 3a00 de51 8051 d7c8 1661 d0bf  .0.&:..Q.Q...a..
-00005a20: b5f4 b421 23c4 b356 9995 bacf 0fa5 bdb8  ...!#..V........
-00005a30: 9eb8 0228 0888 055f b2d9 0cc6 24e9 0bb1  ...(..._....$...
-00005a40: 877c 6f2f 114c 6858 ab1d 61c1 3d2d 66b6  .|o/.LhX..a.=-f.
-00005a50: 9041 dc76 0671 db01 bc20 d298 2a10 d5ef  .A.v.q... ..*...
-00005a60: 8985 b171 1fb5 b606 a5e4 bf9f 33d4 b8e8  ...q........3...
-00005a70: a2c9 0778 34f9 000f 8ea8 0996 1898 0ee1  ...x4...........
-00005a80: bb0d 6a7f 2d3d 6d08 976c 6491 015c 63e6  ..j.-=m..ld..\c.
-00005a90: f451 6b6b 6261 6c1c d830 6585 4e00 62f2  .Qkkbal..0e.N.b.
-00005aa0: ed95 066c 7ba5 011b c1f4 0882 57c4 0ff5  ...l{.......W...
-00005ab0: c6d9 b065 50e9 b712 eab8 be8b 7c88 b9fc  ...eP.......|...
-00005ac0: df1d dd62 492d da15 f37c d38c 654c d4fb  ...bI-...|..eL..
-00005ad0: 5861 b24d ce51 b53a 7400 bca3 e230 bbd4  Xa.M.Q.:t....0..
-00005ae0: 41a5 df4a d795 d83d 6dc4 d1a4 fbf4 d6d3  A..J...=m.......
-00005af0: 6ae9 6943 fcd9 6e34 4688 67ad d0b8 60da  j.iC..n4F.g...`.
-00005b00: 732d 0444 e51d 0333 5f4c 0aaa c97c 0ddd  s-.D...3_L...|..
-00005b10: 3c71 0550 aa41 0227 1010 0bbe 8620 0cc9  <q.P.A.'..... ..
-00005b20: 25b5 6857 b385 6f20 09d4 66b9 9fe4 61ce  %.hW..o ..f...a.
-00005b30: 0ef9 de5e 98c9 d929 2298 d0b0 b4a8 d7c7  ...^...)".......
-00005b40: 173d b359 810d b42e 3b5c bdb7 ad6c bac0  .=.Y....;\...l..
-00005b50: 2083 b8ed b6b3 bf9a 0ce2 b603 9ad2 b174   ..............t
-00005b60: 3947 d5ea af77 d29d 1526 db04 8316 dc73  9G...w...&.....s
-00005b70: 120b 63e3 843b 6494 3e6a 6d0d a85a 6a7a  ..c..;d.>jm..Zjz
-00005b80: 0bcf 0ee4 9dff 0993 27ae 000a b19e 077d  ........'......}
-00005b90: 4493 0ff0 d2a3 0887 68f2 011e fec2 0669  D.......h......i
-00005ba0: 5d57 62f7 cb67 6580 7136 6c19 e706 6b6e  ]Wb..ge.q6l...kn
-00005bb0: 761b d4fe e02b d389 5a7a da10 cc4a dd67  v....+..Zz...J.g
-00005bc0: 6fdf b9f9 f9ef be8e 43be b717 d58e b060  o.......C......`
-00005bd0: e8a3 d6d6 7e93 d1a1 c4c2 d838 52f2 df4f  ....~......8R..O
-00005be0: f167 bbd1 6757 bca6 dd06 b53f 4b36 b248  .g..gW.....?K6.H
-00005bf0: da2b 0dd8 4c1b 0aaf f64a 0336 607a 0441  .+..L....J.6`z.A
-00005c00: c3ef 60df 55df 67a8 ef8e 6e31 79be 6946  ..`.U.g...n1y.iF
-00005c10: 8cb3 61cb 1a83 66bc a0d2 6f25 36e2 6852  ..a...f...o%6.hR
-00005c20: 9577 0ccc 0347 0bbb b916 0222 2f26 0555  .w...G....."/&.U
-00005c30: be3b bac5 280b bdb2 925a b42b 046a b35c  .;..(....Z.+.j.\
-00005c40: a7ff d7c2 31cf d0b5 8b9e d92c 1dae de5b  ....1......,...[
-00005c50: b0c2 649b 26f2 63ec 9ca3 6a75 0a93 6d02  ..d.&.c...ju..m.
-00005c60: a906 099c 3f36 0eeb 8567 0772 1357 0005  ....?6...g.r.W..
-00005c70: 824a bf95 147a b8e2 ae2b b17b 381b b60c  .J...z...+.{8...
-00005c80: 9b8e d292 0dbe d5e5 b7ef dc7c 21df db0b  ...........|!...
-00005c90: d4d2 d386 42e2 d4f1 f8b3 dd68 6e83 da1f  ....B......hn...
-00005ca0: cd16 be81 5b26 b9f6 e177 b06f 7747 b718  ....[&...w.owG..
-00005cb0: e65a 0888 706a 0fff ca3b 0666 5c0b 0111  .Z..pj...;.f\...
-00005cc0: ff9e 658f 69ae 62f8 d3ff 6b61 45cf 6c16  ..e.i.b...kaE.l.
-00005cd0: 78e2 0aa0 eed2 0dd7 5483 044e c2b3 0339  x.......T..N...9
-00005ce0: 6126 67a7 f716 60d0 4d47 6949 db77 6e3e  a&g...`.MGiI.wn>
-00005cf0: 4a6a d1ae dc5a d6d9 660b df40 f03b d837  Jj...Z..f..@.;.7
-00005d00: 53ae bca9 c59e bbde 7fcf b247 e9ff b530  S..........G...0
-00005d10: 1cf2 bdbd 8ac2 baca 3093 b353 a6a3 b424  ........0..S...$
-00005d20: 0536 d0ba 9306 d7cd 2957 de54 bf67 d923  .6......)W.T.g.#
-00005d30: 2e7a 66b3 b84a 61c4 021b 685d 942b 6f2a  .zf..Ja...h].+o*
-00005d40: 37be 0bb4 a18e 0cc3 1bdf 055a 8def 022d  7..........Z...-
-00005d50: 496e 2045 7665 7279 2044 7265 616d 2048  In Every Dream H
-00005d60: 6f6d 6520 6120 4865 6172 7461 6368 6500  ome a Heartache.
-00005d70: b79d 2254 7363 616d 702d 3133 3300 0000  .."Tscamp-133...
-00005d80: 0600 0100 0200 0700 0a00 0300 7502 0300  ............u...
-00005d90: 0200 0300 0100 0500 1700 1400 f17c fe01  .............|..
-00005da0: f1bc fe01 f27c fe01 f2bc fe01 f47c fe01  .....|.......|..
-00005db0: f4bc fe01 f87c fe01 f8bc fe01 f1fc 0100  .....|..........
-00005dc0: f2fc 0100 f4fc 0100 f8fc 0100 0000 0000  ................
-00005dd0: 0000 0000 0000 0000 0000 0000 adde adde  ................
-00005de0: 1000 0000 0400 0000 0400 0000 0400 0000  ................
-00005df0: fa00 0000 b80b 0000 f401 0000 fa00 0000  ................
-00005e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005e20: 0010 2030 4014 2434 4454 6474 0111 2131  .. 0@.$4DTdt..!1
-00005e30: 4151 2535 4555 6575 0212 2232 4252 6236  AQ%5EUeu.."2BRb6
-00005e40: 4656 6676 0313 2333 4353 6373 4757 6777  FVfv..#3CScsGWgw
-00005e50: 4014 2434 4454 6474 0010 2030 4151 2535  @.$4DTdt.. 0AQ%5
-00005e60: 4555 6575 0111 2131 4252 6236 4656 6676  EUeu..!1BRb6FVfv
-00005e70: 0212 2232 4353 6373 4757 6777 0313 2333  .."2CScsGWgw..#3
-00005e80: 4454 6474 0010 2030 4014 2434 4555 6575  DTdt.. 0@.$4EUeu
-00005e90: 0111 2131 4151 2535 4656 6676 0212 2232  ..!1AQ%5FVfv.."2
-00005ea0: 4252 6236 4757 6777 0313 2333 4353 6373  BRb6GWgw..#3CScs
-00005eb0: 0000 0000 0000 0000 0000 0000 0100 0000  ................
-00005ec0: 0900 0000 0000 0000 0000 0000 0000 0000  ................
-00005ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005f00: 0000 0000 0000 0000                      ........
+00001930: 414c 0f22 c034 0721 a068 1202 0903 03f0  AL.".4.!.h......
+00001940: 88ec a068 2900 fff7 5eff 70bd f8b5 050e  ...h)...^.p.....
+00001950: 0002 0f02 000a 0e0e 3f0a 0090 0021 3800  ........?....!8.
+00001960: fff7 0cff 2c00 03e0 2000 fff7 b7ff 641c  ....,... .....d.
+00001970: 2000 3040 a842 f7d0 0098 3900 fff7 d2ff   .0@.B....9.....
+00001980: f8bd 10b5 0400 0800 0021 fff7 f7fe 0022  .........!....."
+00001990: 0121 2000 fff7 0eff 10bd f8b5 0103 0d0f  .! .............
+000019a0: 0104 234b 0e0e 1b68 0706 0021 3f0e 0a00  ..#K...h...!?...
+000019b0: 0120 9c46 0ee0 214b 0124 1b5c 3340 bb42  . .F..!K.$.\3@.B
+000019c0: 00d0 0024 2300 8340 1943 1e4b 1b5c 9c40  ...$#..@.C.K.\.@
+000019d0: 2243 401c 6045 eed3 1948 144c 2b00 03f0  "C@.`E...H.L+...
+000019e0: 74ec 0e08 0a0c 1d15 171d 1d1d 1d1d 1d1d  t...............
+000019f0: 1d14 1548 06e0 1548 04e0 3006 0243 1448  ...H...H..0..C.H
+00001a00: 3b06 1943 0023 03f0 edfc f8bd c161 00e0  ;..C.#.......a..
+00001a10: 8161 1119 7120 4006 8160 f8bd 1300 0a00  .a..q @..`......
+00001a20: 2900 0320 fff7 3dff f8bd 0000 0000 c05e  ).. ..=........^
+00001a30: 0801 4000 0070 00e5 007f 00e5 5807 4000  ..@..p......X.@.
+00001a40: 4000 00e2 6c07 4000 2509 0000 8309 0000  @...l.@.%.......
+00001a50: 4d09 0000 0a00 0100 2120 4004 10b5 03f0  M.......! @.....
+00001a60: 40e9 0028 03d1 ff49 c86a 401c c862 10bd  @..(...I.j@..b..
+00001a70: 0243 70b5 0d00 1400 1000 03f0 22eb 0121  .Cp........."..!
+00001a80: 0904 2043 6a18 0100 2120 4004 03f0 28e9  .. Cj...! @...(.
+00001a90: 0028 03d1 f349 c86a 401c c862 70bd 70b5  .(...I.j@..bp.p.
+00001aa0: 0500 f14c aa02 d60f 2279 c002 c00e 022a  ...L...."y.....*
+00001ab0: 16d1 a279 8242 13d1 2069 8842 10d1 216a  ...y.B.. i.B..!j
+00001ac0: e069 04f0 f5fb 607a b042 06d0 6672 2078  .i....`z.B..fr x
+00001ad0: 6169 4200 8018 0818 6061 0120 a581 a072  aiB.....`a. ...r
+00001ae0: 70bd 70b5 0500 e04c 0e00 2179 c002 c00e  p.p....L..!y....
+00001af0: 0229 0ed1 a179 8142 0bd1 2069 b042 08d1  .)...y.B.. i.B..
+00001b00: 216a e069 04f0 d4fb 0020 a081 2071 0320  !j.i..... .. q. 
+00001b10: a072 2a02 0520 120a 3100 0006 fff7 a8ff  .r*.. ..1.......
+00001b20: 70bd d049 4a68 521c 4a60 0021 8181 0121  p..IJhR.J`.!...!
+00001b30: c170 0221 8172 8e21 0172 7047 8172 c949  .p.!.r.!.rpG.r.I
+00001b40: 086b 401c 0863 7047 f3b5 4022 83b0 0d1d  .k@..cpG..@"....
+00001b50: 087a 8e88 1043 0872 c34c 0020 c880 a079  .z...C.r.L. ...y
+00001b60: c249 401c c006 c00e a071 497b 0022 4f07  .I@......qI{."O.
+00001b70: 7f0f 7901 0818 0290 311d 2800 fff7 d0ed  ..y.....1.(.....
+00001b80: c043 010a a970 0121 e870 0800 b840 0006  .C...p.!.p...@..
+00001b90: 000e 2070 0190 0020 6070 0398 2061 a81c  .. p... `p.. a..
+00001ba0: 6061 a819 401c a061 0020 e070 6072 b048  `a..@..a. .p`r.H
+00001bb0: 2171 0068 e071 ab4d 8b20 2072 2869 401c  !q.h.q.M.  r(i@.
+00001bc0: 2861 0299 3002 0026 4718 0020 a072 a948  (a..0..&G.. .r.H
+00001bd0: 0222 2100 03f0 a4fb 0028 e061 06d0 4169  ."!......(.a..Ai
+00001be0: 2162 a349 0969 04f0 95fb 05e0 ff22 5632  !b.I.i......."V2
+00001bf0: 0020 a1a1 04f0 02fb 0120 0399 3a00 0006  . ....... ..:...
+00001c00: fff7 36ff a07a 0028 fcd0 a07a 0128 0cd1  ..6..z.(...z.(..
+00001c10: 207a 8028 5bd1 0220 2071 0199 0120 8840   z.([..  q... .@
+00001c20: 401e 0504 2d0c a581 0ae0 a868 401c a860  @...-......h@..`
+00001c30: e079 6862 e079 0028 48d0 401e e071 c4e7  .yhb.y.(H.@..q..
+00001c40: 0026 20e0 6069 7100 7118 4718 e807 11d0  .& .`iq.q.G.....
+00001c50: 6079 617a 4007 0907 4018 3106 4018 b978  `yaz@...@.1.@..x
+00001c60: 0904 4018 7978 0902 4018 3978 4018 0399  ..@.yx..@.9x@...
+00001c70: fff7 f0fe a069 b842 02d8 0120 e070 05e0  .....i.B... .p..
+00001c80: 6d08 03d0 761c 0198 8642 dbd3 0020 a072  m...v....B... .r
+00001c90: 0200 7c48 2100 03f0 43fb 0028 07d0 e061  ..|H!...C..(...a
+00001ca0: 4169 2162 7249 4969 04f0 34fb 05e0 ff22  Ai!brIIi..4...."
+00001cb0: 9c32 0020 70a1 04f0 a1fa a07a 0028 fcd0  .2. p......z.(..
+00001cc0: e078 a589 0028 bbd0 002d b9d1 207a 05b0  .x...(...-.. z..
+00001cd0: f0bd 10b5 0400 0078 0128 0bd1 6148 0168  .......x.(..aH.h
+00001ce0: 491c 0160 2079 0028 05d1 a069 04f0 acf8  I..` y.(...i....
+00001cf0: 0020 2070 10bd 401e 2071 a079 e178 4005  .  p..@. q.y.x@.
+00001d00: 0904 4018 2189 4218 0320 e168 0006 fff7  ..@.!.B.. .h....
+00001d10: affe 5d48 0022 2100 03f0 02fb 0028 07d0  ..]H."!......(..
+00001d20: e061 4169 2162 5249 8969 04f0 f3fa 10bd  .aAi!bRI.i......
+00001d30: ff22 d332 0020 50a1 04f0 60fa 10bd c202  .".2. P...`.....
+00001d40: 70b5 d40e 484a 0306 1579 1b0e 012d 11d1  p...HJ...y...-..
+00001d50: 9579 a542 0ed1 1469 8c42 0bd1 8d2b 09d0  .y.B...i.B...+..
+00001d60: 0002 400f 5071 0120 1372 9072 116a d069  ..@.Pq. .r.r.j.i
+00001d70: 04f0 9efa 70bd f3b5 0102 0006 000e 83b0  ....p...........
+00001d80: 090c c506 ed0e 0291 4109 0190 0120 8840  ........A.... .@
+00001d90: 0090 0299 ff20 1930 8142 02d8 0098 1028  ..... .0.B.....(
+00001da0: 0bd9 2a04 0120 0499 8c32 4006 fff7 60fe  ..*.. ...2@...`.
+00001db0: 2c49 086a 401c 0862 89e7 2b4c 0826 2434  ,I.j@..b..+L.&$4
+00001dc0: 0027 2078 0128 23d1 e068 0499 8842 22d1  .' x.(#..h...B".
+00001dd0: e078 a842 1fd1 216a e069 04f0 69fa 2148  .x.B..!j.i..i.!H
+00001de0: 816a 491c 8162 2804 b905 4218 0120 0499  .jI..b(...B.. ..
+00001df0: 8032 4006 fff7 3cfe 1d4d 0022 6868 2071  .2@...<..M."hh q
+00001e00: 2148 2100 03f0 8cfa 0028 7bd1 1f4a 82e0  !H!......({..J..
+00001e10: 0028 00d1 3e00 2434 7f1c 082f d1d3 082e  .(..>.$4.../....
+00001e20: 0ad1 2a04 0499 8d32 b005 fff7 21fe 0d49  ..*....2....!..I
+00001e30: 8869 401c 8861 4ae7 2420 0b49 7043 2431  .i@..aJ.$ .IpC$1
+00001e40: 4418 04f0 11f8 0028 22d1 2a04 0120 0499  D......(".*.. ..
+00001e50: 8d32 4006 fff7 0cfe 0249 c869 401c c861  .2@......I.i@..a
+00001e60: 35e7 0000 7402 4000 3001 4000 007f 00e5  5...t.@.0.@.....
+00001e70: 0000 4000 3d0b 0000 7363 616d 702d 7032  ..@.=...scamp-p2
+00001e80: 702e 6300 230b 0000 d30c 0000 2602 0000  p.c.#.......&...
+00001e90: 0121 a061 2170 019a 6271 049a e260 e570  .!.a!p..bq...`.p
+00001ea0: 009a 6270 0022 a270 a271 009a 9140 491e  ..bp.".p.q...@I.
+00001eb0: 6181 801d 2181 2061 0299 4118 491e 6161  a...!. a..A.I.aa
+00001ec0: 0299 2038 8177 0299 090a c177 2804 7105  .. 8.w.....w(.q.
+00001ed0: 4218 0120 0499 8032 4006 fff7 c9fd 8d4d  B.. ...2@......M
+00001ee0: 8d49 6868 2071 b000 4018 026c 521c 0264  .Ihh q..@..lR..d
+00001ef0: 4869 0022 401c 4861 8848 2100 03f0 10fa  Hi."@.Ha.H!.....
+00001f00: 0028 06d0 e061 4169 2162 a969 04f0 02fa  .(...aAi!b.i....
+00001f10: dde6 2722 1201 8249 0020 04f0 6ff9 d6e6  ..'"...I. ..o...
+00001f20: 70b5 0400 7c48 0d00 c168 491c c160 2079  p...|H...hI..` y
+00001f30: 0028 05d1 a069 03f0 87ff 0020 2070 70bd  .(...i.....  pp.
+00001f40: 401e 2071 e178 6805 0904 4218 0120 e168  @. q.xh...B.. .h
+00001f50: 8006 fff7 8dfd 7348 2a00 2100 03f0 e0f9  ......sH*.!.....
+00001f60: 0028 07d0 e061 4169 2162 6a49 c969 04f0  .(...aAi!bjI.i..
+00001f70: d1f9 70bd 6c4a 6a49 0020 04f0 3ff9 70bd  ..p.lJjI. ..?.p.
+00001f80: 0202 520f 2423 5a43 684b 10b5 d418 2278  ..R.$#ZChK...."x
+00001f90: c002 c00e 022a 0fd1 e278 8242 0cd1 e068  .....*...x.B...h
+00001fa0: 8842 09d1 0020 2070 216a e069 04f0 80f9  .B...  p!j.i....
+00001fb0: a069 0021 02f0 49f8 10bd f8b5 2423 460f  .i.!..I.....$#F.
+00001fc0: 7343 5a4c c200 1c19 2378 d20f 012b 6cd1  sCZL....#x...+l.
+00001fd0: e368 8b42 69d1 a179 9142 66d1 6178 020e  .h.Bi..y.Bf.ax..
+00001fe0: 491e 0a40 2169 5300 d318 c918 030a 0870  I..@!iS........p
+00001ff0: 000c 4b70 0127 8870 3800 9040 2289 8243  ..Kp.'.p8..@"..C
+00002000: 2281 6269 8a42 04d8 2189 401e 0140 2181  ".bi.B..!.@..@!.
+00002010: a770 2089 0028 48d1 216a e069 04f0 48f9  .p ..(H.!j.i..H.
+00002020: a078 3c4d 0028 1bd0 0220 2070 e868 2071  .x<M.(...  p.h q
+00002030: e178 7005 0904 4218 0120 e168 8006 fff7  .xp...B.. .h....
+00002040: 17fd 3848 3200 2100 03f0 6af9 0028 04d0  ..8H2.!...j..(..
+00002050: e061 4169 2162 e969 25e0 334a 5032 27e0  .aAi!b.i%.3JP2'.
+00002060: a079 7840 a071 6178 2269 4b00 c918 5118  .yx@.qax"iK...Q.
+00002070: 2161 6189 2181 e178 4005 0904 4018 2189  !aa.!..x@...@.!.
+00002080: 4218 0320 e168 0006 fff7 f2fc a868 2071  B.. .h.......h q
+00002090: 2248 0022 2100 03f0 43f9 0028 06d0 e061  "H."!...C..(...a
+000020a0: 4169 2162 a969 04f0 35f9 f8bd 1e4a 6832  Ai!b.i..5....Jh2
+000020b0: 1b49 0020 04f0 a2f8 f8bd 70b5 0400 0d00  .I. ......p.....
+000020c0: 02f0 feef 0028 07d1 2001 000f 0128 04d1  .....(.. ....(..
+000020d0: 2900 2000 fff7 4ffe 70bd 0228 04d1 2900  ). ...O.p..(..).
+000020e0: 2000 fff7 2cfe 70bd 0328 04d1 2900 2000   ...,.p..(..). .
+000020f0: fff7 d5fc 70bd 0428 04d1 2900 2000 fff7  ....p..(..). ...
+00002100: f0fc 70bd 0528 fcd1 2900 2000 fff7 38ff  ..p..(..). ...8.
+00002110: 70bd 0000 0000 4000 7402 4000 d30c 0000  p.....@.t.@.....
+00002120: 780e 0000 210f 0000 9602 0000 5401 4000  x...!.......T.@.
+00002130: fa48 fb49 007a 8870 f848 fa49 a030 8069  .H.I.z.p.H.I.0.i
+00002140: 0861 f948 4860 0021 0b00 1a00 0f29 01d0  .a.HH`.!.....)..
+00002150: 0200 1432 0260 1430 491c 1029 f5d3 7047  ...2.`.0I..)..pG
+00002160: f0b5 f248 0068 050a 0206 f148 120e 0068  ...H.h.....H...h
+00002170: 040a 0306 ef48 1b0e 0168 080a 281a 00e0  .....H...h..(...
+00002180: 0c30 0028 fcdb 00e0 0c38 0c28 fcda 0906  .0.(.....8.(....
+00002190: 090e 511a 00e0 0c31 0029 fcdb 00e0 0c39  ..Q....1.).....9
+000021a0: 0c29 fcda 0c26 7143 de4e 1436 8919 085c  .)...&qC.N.6...\
+000021b0: 0707 0609 3f0f a81b 00d5 0019 d11b 00d5  ....?...........
+000021c0: c918 d64b 0002 3202 4018 d449 d219 8033  ...K..2.@..I...3
+000021d0: 2039 da83 8880 0881 f0bd f0b5 030a 0406   9..............
+000021e0: 240e 0020 0626 4100 711a 0422 8a40 521e  $.. .&A.q..".@R.
+000021f0: 1d00 cd40 ad07 ad0f 2700 cf40 b907 090f  ...@....'..@....
+00002200: 6d18 d243 1900 1140 2240 1218 0906 1204  m..C...@"@......
+00002210: 8918 0122 aa40 8918 8201 c74d 401c 0428  ...".@.....M@..(
+00002220: a950 e0d3 f0bd f0b5 89b0 c048 0068 fff7  .P.........H.h..
+00002230: d4ff 0020 0490 c049 8001 0890 0858 bf49  ... ...I.....X.I
+00002240: 000c 0840 0390 0498 0621 4000 091a 0120  ...@.....!@.... 
+00002250: 8840 0291 0027 0100 4143 0790 0691 0025  .@...'..AC.....%
+00002260: 3802 0590 a800 c019 0190 0598 0299 4019  8.............@.
+00002270: 8840 0024 0090 28e0 0799 029a 491e 2000  .@.$..(.....I. .
+00002280: d040 009b 039a 2140 d218 0902 5118 0e18  .@....!@....Q...
+00002290: a748 0068 8642 17d2 3106 0006 090e 000e  .H.h.B..1.......
+000022a0: 8142 11d2 3000 03f0 07fb 0628 0cd0 a248  .B..0......(...H
+000022b0: 0899 0818 0199 4900 4118 0e82 019a 0121  ......I.A......!
+000022c0: 8018 2030 0174 03e0 641c 0698 a042 d3d8  .. 0.t..d....B..
+000022d0: 6d1c 042d c6d3 7f1c 042f c0d3 0498 401c  m..-...../....@.
+000022e0: 0428 0490 a7d3 09b0 f0bd 10b5 944c 2379  .(...........L#y
+000022f0: 012b 04d0 2300 0833 07c3 0120 2071 10bd  .+..#..3...  q..
+00002300: 10b5 8f4c 1434 2379 012b 04d0 2300 0833  ...L.4#y.+..#..3
+00002310: 07c3 0120 2071 10bd ffb5 81b0 0500 1600  ...  q..........
+00002320: 874c 0020 2071 8804 0521 4905 4018 2a00  .L.  q...!I.@.*.
+00002330: 0021 02f0 d6ec 0028 02d1 8f20 05b0 f0bd  .!.....(... ....
+00002340: 8048 0222 211d 02f0 ebff 0500 06d1 ff22  .H."!.........."
+00002350: 2f32 7da1 03f0 52ff 8a20 efe7 6f69 0499  /2}...R.. ..oi..
+00002360: 2800 03f0 d7ff 2079 0028 fcd0 2079 0228  (..... y.(.. y.(
+00002370: 01d1 8620 e2e7 3900 2800 03f0 99ff 002e  ... ..9.(.......
+00002380: 01d0 e068 3060 8020 d8e7 f8b5 0500 0800  ...h0`. ........
+00002390: 6b4c 1f00 0021 1434 2171 1168 5122 8004  kL...!.4!q.hQ"..
+000023a0: 5204 8018 2a00 02f0 9cec 0028 01d1 8f20  R...*......(... 
+000023b0: f8bd 6448 0222 211d 02f0 b2ff 0500 06d1  ..dH."!.........
+000023c0: ff22 5132 60a1 03f0 19ff 8a20 f8bd 6e69  ."Q2`...... ..ni
+000023d0: 3900 2800 03f0 9eff 2279 002a fcd0 2079  9.(....."y.*.. y
+000023e0: 0228 01d1 8620 f8bd 3100 2800 03f0 60ff  .(... ..1.(...`.
+000023f0: 8020 f8bd 4b4a 5068 0028 08d0 0168 5160  . ..KJPh.(...hQ`
+00002400: 9168 491c 9160 d368 9942 00d9 d160 7047  .hI..`.h.B...`pG
+00002410: 4449 4a68 0260 4860 8868 401e 8860 7047  DIJh.`H`.h@..`pG
+00002420: 3e49 2039 c879 401c 7f28 00d9 0120 c871  >I 9.y@..(... .q
+00002430: 4000 7047 3949 4031 8879 401c 7f28 00d9  @.pG9I@1.y@..(..
+00002440: 0120 8871 4000 7047 0006 410e 4809 c906  . .q@.pG..A.H...
+00002450: c90e 0122 8a40 8100 10b5 314c 801c 0919  ...".@....1L....
+00002460: 8b6a 8007 1343 8b62 0021 000f 0019 8162  .j...C.b.!.....b
+00002470: 10bd ffb5 81b0 0400 002b 02d0 fff7 d0ff  .........+......
+00002480: 0443 f820 1040 5507 0090 0299 6d0f 160a  .C. .@U.....m...
+00002490: 2000 02f0 12ee 2043 0127 0190 0024 2d49   ..... C.'...$-I
+000024a0: 3800 a040 0968 3040 0842 0ad0 0098 02f0  8..@.h0@.B......
+000024b0: 1dfe 4121 a004 4904 4018 019a 0299 02f0  ..A!..I.@.......
+000024c0: 10ec 641c 062c ead3 6d1e e7d2 36e7 f1b5  ..d..,..m...6...
+000024d0: 0b22 1206 82b0 fff7 adff 0400 1443 0299  ."...........C..
+000024e0: 2000 02f0 eaed 2043 1a4f 0725 0024 0126   ..... C.O.%.$.&
+000024f0: 0190 3000 a040 3968 2840 0842 0ad0 0820  ..0..@9h(@.B... 
+00002500: 02f0 f4fd 4121 a004 4904 4018 019a 0299  ....A!..I.@.....
+00002510: 02f0 e6eb 641c 062c ebd3 febd 207f 00e5  ....d..,.... ...
+00002520: 3805 4000 2000 4000 f802 4000 d400 4000  8.@. .@...@...@.
+00002530: d800 4000 dc00 4000 3804 4000 fcfc 0000  ..@...@.8.@.....
+00002540: 3007 4000 cf2d 0000 7363 616d 702d 6e6e  0.@..-..scamp-nn
+00002550: 2e63 0000 e400 4000 f8b5 f948 0168 f94a  .c....@....H.h.J
+00002560: 9142 1dd0 f849 0b68 9342 19d0 0068 0524  .B...I.h.B...h.$
+00002570: 2406 0704 0868 0004 000c 0743 3900 2000  $....h.....C9. .
+00002580: 02f0 9aed 2043 0600 0024 4125 6d04 a004  .... C...$A%m...
+00002590: 4019 3200 3900 02f0 a4eb 641c 062c f6d3  @.2.9.....d..,..
+000025a0: f8bd f8b5 0704 0804 000c e84c 0743 3900  ...........L.C9.
+000025b0: 2000 02f0 82ed 2043 0600 0024 4125 6d04   ..... C...$A%m.
+000025c0: a004 4019 3200 3900 02f0 8aeb 641c 062c  ..@.2.9.....d..,
+000025d0: f6d3 f8bd f8b5 de48 dc4c 0068 241d 0706  .......H.L.h$...
+000025e0: dc48 0068 0006 000a 0743 db48 0068 0006  .H.h.....C.H.h..
+000025f0: 000c 0743 d948 0068 0006 000e 0743 3900  ...C.H.h.....C9.
+00002600: 2000 02f0 5aed 2043 0600 0024 4125 6d04   ...Z. C...$A%m.
+00002610: a004 4019 3200 3900 02f0 62eb 641c 062c  ..@.2.9...b.d..,
+00002620: f6d3 f8bd feb5 ce49 ce4b 0868 4206 401c  .......I.K.hB.@.
+00002630: 0860 cd48 120e 0068 d418 0004 0100 0090  .`.H...h........
+00002640: 2000 02f0 3aed 2043 c84e 0024 0125 4127   ...:. C.N.$.%A'
+00002650: 7f04 0190 2800 3168 a040 0842 05d0 a004  ....(.1h.@.B....
+00002660: 019a 0099 c019 02f0 3ceb 641c 062c f1d3  ........<.d..,..
+00002670: 53e7 0a04 0b0c be49 120c 30b4 1c04 00d5  S......I..0.....
+00002680: 0b43 1404 00d5 0a43 ba49 0956 c918 b94b  .C.....C.I.V...K
+00002690: 0833 1856 b84b 8018 ca1d f832 9a42 50d2  .3.V.K.....2.BP.
+000026a0: fe22 d243 9042 4cdb ff28 4adc b34a d279  .".C.BL..(J..J.y
+000026b0: d207 0fd0 0829 44d2 0828 42da 0028 40db  .....)D..(B..(@.
+000026c0: 0c22 a74b 4243 1433 d218 525c 0b01 1b18  .".KBC.3..R\....
+000026d0: 9a42 36d1 9a4c 0022 2368 002b 01da 0029  .B6..L."#h.+...)
+000026e0: 0dda 2568 cb0f ed0f ab42 0ad1 2368 0d1e  ..%h.....B..#h..
+000026f0: 00da 4d42 002b 00da 5b42 9d42 01da 2160  ..MB.+..[B.B..!`
+00002700: 0122 914d 2968 0029 01da 0028 0dda 2b68  .".M)h.)...(..+h
+00002710: c10f db0f 9942 0bd1 2968 031e 00da 4342  .....B..)h....CB
+00002720: 0029 00da 4942 8b42 02da 2860 0220 0243  .)..IB.B..(`. .C
+00002730: 002a 06d0 9249 0020 0860 2968 2068 30bc  .*...I. .`)h h0.
+00002740: 2fe7 30bc 7047 080c 0904 894a 090c f0b4  /.0.pG.....J....
+00002750: 0304 00d5 1043 0b04 00d5 1143 864b c21d  .....C.....C.K..
+00002760: f832 9a42 1fd2 fe22 d243 9142 1bdb ff29  .2.B...".C.B...)
+00002770: 19dc 0123 4202 5b04 d318 ca1d f932 1343  ...#B.[......2.C
+00002780: dc08 804a 5e07 1568 760f 0123 2a5d b340  ...J^..hv..#*].@
+00002790: 1343 1b06 1b0e 9a42 2b55 04d0 784b 0022  .C.....B+U..xK."
+000027a0: 1a60 f0bc fde6 f0bc 7047 0a02 ff23 080e  .`......pG...#..
+000027b0: 120e db43 f0b4 0028 00d0 1843 002a 00d0  ...C...(...C.*..
+000027c0: 1a43 634d 0b04 1b0e 0c06 2e68 240e 0021  .CcM.......h$..!
+000027d0: b042 01da 2860 0121 5e48 0568 aa42 01da  .B..(`.!^H.h.B..
+000027e0: 0260 0121 5c48 0268 9342 01dd 0360 0121  .`.!\H.h.B...`.!
+000027f0: 5a48 0268 9442 01dd 0460 01e0 0029 d2d0  ZH.h.B...`...)..
+00002800: 6149 0020 0860 f0bc 0100 e3e6 cbe7 1307  aI. .`..........
+00002810: 9b0f 04d0 012b 03d0 022b 02d1 c5e7 28e7  .....+...+....(.
+00002820: 91e7 7047 0022 1100 8306 10b5 03d5 010e  ..pG."..........
+00002830: 0906 ff22 1206 c306 05d5 ff24 2404 0300  ...".......$$...
+00002840: 2340 1943 2243 0307 05d5 0124 e403 0300  #@.C"C.....$....
+00002850: 2340 1943 2243 4307 05d5 1f24 2402 0300  #@.C"CC....$$...
+00002860: 2340 1943 2243 8307 03d5 c023 1840 0143  #@.C"C.....#.@.C
+00002870: 1a43 e123 1b06 1868 9043 0843 1860 10bd  .C.#...h.C.C.`..
+00002880: 424a 030f 10b5 02f0 20ed 0604 0c0f 1728  BJ...... ......(
+00002890: 2f31 3a4b 010a 403b 1972 9170 5872 d070  /1:K..@;.r.pXr.p
+000028a0: 24e0 03f0 a7fa 21e0 0107 3448 090f 6038  $.....!...4H..`8
+000028b0: c173 0021 0162 19e0 1169 8142 01d1 0020  .s.!.b...i.B... 
+000028c0: 10bd 1061 c007 01d0 ff21 00e0 0021 2f48  ...a.....!...!/H
+000028d0: 1022 2830 02f0 e6ec 08e0 0022 2c48 1100  ."(0.......",H..
+000028e0: 1300 02f0 7ffd 01e0 fff7 57f8 0120 10bd  ..........W.. ..
+000028f0: 0a03 10b5 940f 8a03 930f 204a 603a 012b  .......... J`:.+
+00002900: 02d1 e522 1206 09e0 022b 02d1 7122 5206  ...".....+..q"R.
+00002910: 04e0 032b 02d1 194a 203a 126a 0904 090e  ...+...J :.j....
+00002920: 8918 002c 01d1 0870 10bd 012c 01d1 0880  ...,...p...,....
+00002930: 10bd 0860 10bd 0a02 120f 2bd1 d8e7 0000  ...`......+.....
+00002940: 1801 4000 00fc ffff 1c01 4000 0400 0005  ..@.......@.....
+00002950: 2001 4000 2801 4000 2401 4000 2c01 4000   .@.(.@.$.@.,.@.
+00002960: 2000 4000 0000 3f08 d400 4000 e400 4000   .@...?...@...@.
+00002970: 0000 ffff d853 0000 ff01 0000 607f 00e5  .....S......`...
+00002980: 1001 4000 ec00 4000 1401 4000 3805 4000  ..@...@...@.8.@.
+00002990: 2712 0000 7047 feb5 8446 0c00 a505 1100  '...pG...F......
+000029a0: 200c ad0d 8200 ff4b 0192 1b69 0093 9a58   ......K...i...X
+000029b0: fd4e 130e 9e46 1304 3268 0127 bf02 2600  .N...F..2h.'..&.
+000029c0: 1b0c 3e43 9042 1bd0 f445 01d1 9d42 17d2  ..>C.B...E...B..
+000029d0: f64f 0122 3f68 8a40 3a42 11d0 f44a 9342  .O."?h.@:B...J.B
+000029e0: 03d1 f44b 5a88 521c 5a80 6246 009f 019b  ...KZ.R.Z.bF....
+000029f0: 1206 5219 fa50 02f0 87ff ef48 8542 00d3  ..R..P.....H.B..
+00002a00: 3400 601c 89e5 70b5 0025 ea4a eb4c 203a  4.`...p..%.J.L :
+00002a10: 9268 2262 a061 0802 400e 2071 080a 6071  .h"b.a..@. q..`q
+00002a20: a571 2000 6572 2022 2900 4830 6570 02f0  .q .er ").H0ep..
+00002a30: 3aec 2000 2022 0021 8830 02f0 34ec e048  :. . ".!.0..4..H
+00002a40: e561 0563 4563 a169 0123 0804 090c 8a07  .a.cEc.i.#......
+00002a50: 000c 920f 0028 08d0 9501 e21f f93a 5259  .....(.......:RY
+00002a60: 150c 8d42 02d1 0242 00d0 6372 2370 70bd  ...B...B..cr#pp.
+00002a70: feb5 0404 8f03 050c 810b bf0b 8004 3843  ..............8C
+00002a80: 0090 cf48 0191 436b 026b 0098 ae07 240c  ...H..Ck.k....$.
+00002a90: b60f 121a 8b41 01d3 0120 3ee5 c848 009a  .....A... >..H..
+00002aa0: 0263 002c 4163 07d0 c648 b101 4058 010c  .c.,Ac...H..@X..
+00002ab0: a942 07d1 2042 05d0 c048 0121 4172 c169  .B.. B...H.!Ar.i
+00002ac0: 3943 c161 0020 28e5 f8b5 bc4c 2379 8342  9C.a. (....L#y.B
+00002ad0: 0fd1 2078 0128 0cd1 1002 000e 4509 c606  .. x.(......E...
+00002ae0: f60e 0123 b340 ad00 2e19 b56c 2f00 1f42  ...#.@.....l/..B
+00002af0: 01d0 0020 f8bd 1d43 b564 6162 6161 1104  ... ...C.dabaa..
+00002b00: 090e 491c a181 e071 0020 0100 e081 ab48  ..I....q. .....H
+00002b10: 2022 6830 02f0 c6eb 0220 2070 0120 f8bd   "h0.....  p. ..
+00002b20: 1302 70b5 1c0e a54b 1d79 8542 12d1 d879  ..p....K.y.B...y
+00002b30: a042 0fd1 1878 0228 0cd1 1004 000e 4409  .B...x.(......D.
+00002b40: c506 ed0e 0122 aa40 a400 e518 ac6e 2600  .....".@.....n&.
+00002b50: 1642 01d0 0020 70bd de89 8000 761c 1443  .B... p.....v..C
+00002b60: c018 de81 c030 ac66 c162 5869 4018 5861  .....0.f.bXi@.Xa
+00002b70: 0120 70bd 70b5 1202 904d 120e 2b79 8342  . p.p....M..+y.B
+00002b80: 12d1 e879 9042 0fd1 2878 0228 0cd1 5009  ...y.B..(x.(..P.
+00002b90: d206 0126 d20e 3400 9440 8000 4219 8032  ...&..4..@..B..2
+00002ba0: 9068 0300 2342 01d0 0020 70bd 2043 9060  .h..#B... p. C.`
+00002bb0: 6869 4018 6861 0dd1 e989 a889 8142 09d1  hi@.ha.......B..
+00002bc0: a979 8200 491c a971 7d49 686a d439 02f0  .y..I..q}Ihj.9..
+00002bd0: 40eb 00e0 6e70 0120 2e70 70bd 774b 10b5  @...np. .pp.wK..
+00002be0: 1a79 8242 02d1 1878 0128 01d0 0020 10bd  .y.B...x.(... ..
+00002bf0: 0020 1870 5878 0028 14d1 9879 5a79 9042  . .pXx.(...yZy.B
+00002c00: 10d1 587a 0028 0dd0 da69 6f48 0a43 196a  ..Xz.(...ioH.C.j
+00002c10: 0023 02f0 e7fb 0028 04d1 7d22 6b49 d200  .#.....(..}"kI..
+00002c20: 03f0 ecfa 0120 10bd f3b5 81b0 0500 0027  ..... .........'
+00002c30: 4679 c079 7106 00d4 0700 0024 0121 0800  Fy.yq......$.!..
+00002c40: a040 3042 16d0 e019 0628 00d3 801f 574a  .@0B.....(....WJ
+00002c50: 8140 1268 1142 0dd0 a968 8004 0818 2a69  .@.h.B...h....*i
+00002c60: e968 02f0 3ee8 0028 04d1 534a 5749 121d  .h..>..(..SJWI..
+00002c70: 03f0 c4fa 641c 062c e0d3 029a 521e 0cd0  ....d..,....R...
+00002c80: ab79 5348 2900 03f0 7dfb 0028 04d1 4a4a  .ySH)...}..(..JJ
+00002c90: 4e49 0e32 03f0 b2fa 3fe4 2800 fff7 b8fb  NI.2....?.(.....
+00002ca0: 3be4 930f 10b5 13d1 9300 5401 5b0f 640f  ;.........T.[.d.
+00002cb0: 8342 0dd1 8c42 0bd1 d043 3c49 0002 800e  .B...B...C<I....
+00002cc0: 0860 3c49 8039 4871 9003 800b 01f0 55fb  .`<I.9Hq......U.
+00002cd0: 10bd f7b5 0600 3f49 9004 8957 400f 4518  ......?I...W@.E.
+00002ce0: 3c49 5005 0831 8957 400f 1700 4418 082d  <IP..1.W@...D..-
+00002cf0: 72d2 082c 70da 002c 6edb 0c20 2949 6043  r..,p..,n.. )I`C
+00002d00: 1431 4018 405d 2901 0919 8842 64d1 3806  .1@.@])....Bd.8.
+00002d10: 400e 61d0 4209 c106 c90e 0120 8840 274b  @.a.B...... .@'K
+00002d20: 9100 c918 8c46 896b 0b00 0342 54d1 0143  .....F.k...BT..C
+00002d30: 6346 921c 9963 9107 2048 090f 0818 0022  cF...c.. H....."
+00002d40: 8263 019a 2100 2800 fff7 abff 3f20 0002  .c..!.(.....? ..
+00002d50: 8743 e802 3843 2102 0143 0d01 2d09 0199  .C..8C!..C..-...
+00002d60: 2800 02f0 aae9 2843 0400 fff7 43fb 0028  (.....(C....C..(
+00002d70: 02d1 114a 7632 33e0 0121 b140 3f22 5140  ...Jv23..!.@?"Q@
+00002d80: 4171 0021 8171 1349 c671 1031 0a68 019b  Aq.!.q.I.q.1.h..
+00002d90: 0461 c360 8260 0100 0d48 0122 0823 03f0  .a.`.`...H.".#..
+00002da0: f1fa 1ae0 2000 4000 d400 4000 e400 4000  .... .@...@...@.
+00002db0: ffff 0000 e07f 00e5 ff03 0000 3805 4000  ............8.@.
+00002dc0: f806 4000 3804 4000 0708 0000 4815 0000  ..@.8.@.....H...
+00002dd0: 291c 0000 d853 0000 06e0 0028 04d1 674a  )....S.....(..gJ
+00002de0: 6749 0020 03f0 0afa 42e4 f7b5 1000 0d00  gI. ....B.......
+00002df0: 1600 02f0 62e9 0028 04d0 6248 816a 491c  ....b..(..bH.jI.
+00002e00: 8162 35e4 3001 040f 3006 400e 0b2c 05d1  .b5.0...0.@..,..
+00002e10: 0098 3200 2900 fff7 5cff 29e4 052c 05d1  ..2.)...\.)..,..
+00002e20: 0098 3200 2900 fff7 f2fc 21e4 5549 a200  ..2.).....!.UI..
+00002e30: c039 5118 8031 8a6a 521c 072c 8a62 1ad2  .9Q..1.jR..,.b..
+00002e40: 0028 18d0 4309 c206 d20e 0121 9140 4d4a  .(..C......!.@MJ
+00002e50: 9f00 c03a ba18 9446 926a 1700 0f42 d0d1  ...:...F.j...B..
+00002e60: 0a43 6746 9b1c ba62 4649 9a07 c039 0023  .CgF...bFI...9.#
+00002e70: 120f 5118 8b62 2300 02f0 26ea 100a 0e12  ..Q..b#...&.....
+00002e80: 091c 0921 262d 0909 0935 3a3f 4409 b8e7  ...!&-...5:?D...
+00002e90: 2800 fff7 f5fc 39e0 2800 fff7 c3fc 37e0  (.....9.(.....7.
+00002ea0: 3949 086a 801c a842 abd8 6840 a9d4 681e  9I.j...B..h@..h.
+00002eb0: 0862 2de0 3100 2800 fff7 3dfd 28e0 3100  .b-.1.(...=.(.1.
+00002ec0: 2800 fff7 a0fd 23e0 3100 2800 fff7 d0fd  (.....#.1.(.....
+00002ed0: 0028 96d1 1ce0 009a 2900 fff7 5cfd 0500  .(......)...\...
+00002ee0: 4005 8ed4 14e0 3200 2900 fff7 edfd 0de0  @.....2.).......
+00002ef0: 3200 2900 fff7 14fe 08e0 3200 2900 fff7  2.).......2.)...
+00002f00: 39fe 03e0 3200 2900 fff7 68fe 0028 84d0  9...2.)...h..(..
+00002f10: 6007 04d5 1b48 c038 8778 c478 03e0 3002  `....H.8.x.x..0.
+00002f20: 070e 3004 040e 3601 3609 2900 3000 02f0  ..0...6.6.).0...
+00002f30: c4e8 0643 fff7 5efa 0028 02d1 5122 1201  ...C..^..(..Q"..
+00002f40: 17e0 f821 2140 0831 4771 8171 0099 c171  ...!!@.1Gq.q...q
+00002f50: 0e49 0823 0a68 0661 c560 8260 6207 520f  .I.#.h.a.`.`b.R.
+00002f60: 0100 0b48 521c 03f0 0dfa 0028 8fd1 034a  ...HR......(...J
+00002f70: 9b32 0349 0020 03f0 41f9 43e5 8204 0000  .2.I. ..A.C.....
+00002f80: 4815 0000 f805 4000 007f 00e5 f453 0000  H.....@......S..
+00002f90: 291c 0000 10b5 c269 8169 d30f 4069 db07  )......i.i..@i..
+00002fa0: fff7 67fa 0020 10bd f0b5 0600 85b0 4169  ..g.. ........Ai
+00002fb0: 0023 080c 0390 fe20 0140 0291 f849 b069  .#..... .@...I.i
+00002fc0: f769 0840 0299 039a 4018 0321 8906 4018  .i.@....@..!..@.
+00002fd0: 3900 fff7 4efa b069 3500 0104 090e 491c  9...N..i5.....I.
+00002fe0: 0091 ff21 0904 0840 0299 4018 0d21 0906  ...!...@..@..!..
+00002ff0: 4018 2035 0024 0190 09e0 019a 02cd 2002  @. 5.$........ .
+00003000: 8018 039a 7f18 0023 fff7 33fa 641c 0098  .......#..3.d...
+00003010: 8442 f2d3 b069 ff21 0904 0840 0299 039a  .B...i.!...@....
+00003020: 4018 0721 4906 4018 7942 0023 fff7 21fa  @..!I.@.yB.#..!.
+00003030: 0020 05b0 f0bd f3b5 0400 8422 81b0 4169  . ........."..Ai
+00003040: 0802 0e06 000e 360e 0428 01d8 102e 01d3  ......6..(......
+00003050: 2282 6ce0 d34d 0028 02d0 0128 45d1 02e0  ".l..M.(...(E...
+00003060: 00f0 80fe 0600 ff2e 35d0 7001 4519 2022  ........5.p.E. "
+00003070: 0021 2800 02f0 16e9 6169 0801 090d 0f0a  .!(.....ai......
+00003080: 000f 3f02 0028 02d0 411e 0120 8840 0743  ..?..(..A.. .@.C
+00003090: a881 ef81 a069 000c e882 6069 000a 2876  .....i....`i..(v
+000030a0: e069 0028 07d0 2000 1c30 2900 fef7 a8f9  .i.(.. ..0).....
+000030b0: b805 06d5 11e0 b805 0fd4 2900 02a8 fef7  ..........).....
+000030c0: 9ff9 a069 6881 e889 0121 4903 0843 e881  ...ih....!I..C..
+000030d0: 2800 fef7 3afa 6661 23e0 a069 a882 e889  (...:.fa#..i....
+000030e0: 0121 c903 0843 e881 f5e7 0228 0ed1 7001  .!...C.....(..p.
+000030f0: 4119 a069 4501 ff20 0130 8542 a8d8 2000  A..iE.. .0.B.. .
+00003100: 2a00 1430 02f0 50e8 2800 febd 0428 0ad1  *..0..P.(....(..
+00003110: a549 a64a 0868 8018 6061 a069 1028 00d2  .I.J.h..`a.i.(..
+00003120: 0860 0420 febd 0020 7101 4919 c881 0020  .`. ... q.I.... 
+00003130: febd 10b5 0400 9e48 0078 ff28 02d1 9d48  .......H.x.(...H
+00003140: 0088 00e0 9c48 0104 9c48 4268 0068 1202  .....H...HBh.h..
+00003150: 8918 0818 6061 9a48 a061 9a48 9aa1 0068  ....`a.H.a.H...h
+00003160: e061 2000 2030 02f0 5ee8 2000 3030 9aa1  .a . 0..^. .00..
+00003170: 02f0 58e8 2220 10bd f0b5 0500 85b0 8069  ..X." .........i
+00003180: 0290 e869 0190 0298 ff21 0131 8842 02d8  ...i.....!.1.B..
+00003190: 0198 0528 01d9 8420 13e0 8648 2e00 1436  ...(... ...H...6
+000031a0: 2030 807a 6f69 0090 0298 0024 8008 0390   0.zoi.....$....
+000031b0: 0ee0 009b 0199 3200 3800 fff7 adf8 8028  ......2.8......(
+000031c0: 02d0 2882 0020 34e7 0398 3f1d 361d 641c  ..(.. 4...?.6.d.
+000031d0: a042 eed8 0298 2ce7 feb5 0500 8069 e969  .B....,......i.i
+000031e0: 0191 ff21 0131 8842 02d8 0199 0529 01d9  ...!.1.B.....)..
+000031f0: 8420 12e0 6f49 2e00 2036 2031 897a 6f69  . ..oI.. 6 1.zoi
+00003200: 0024 8008 0091 0290 0de0 009b 0199 3200  .$............2.
+00003210: 3800 fff7 baf8 8028 01d0 2882 05e0 0298  8......(..(.....
+00003220: 3f1d 361d 641c a042 efd8 0020 febd 10b5  ?.6.d..B... ....
+00003230: 8169 4069 fef7 e7fa 0020 10bd 10b5 4169  .i@i..... ....Ai
+00003240: ca07 02d0 8421 0182 04e0 5a48 c030 8068  .....!....ZH.0.h
+00003250: fef7 d9fa 0020 10bd 70b5 0400 4169 0806  ..... ..p...Ai..
+00003260: 0a04 000e 130e 090c 0028 03d1 0120 02f0  .........(... ..
+00003270: a9fa 1ce0 8425 0128 03d1 a069 02f0 76fa  .....%.(...i..v.
+00003280: 05e0 0228 07d1 e269 a069 02f0 b5fa 0028  ...(...i.i.....(
+00003290: 0dd1 2582 0be0 0328 fbd1 a069 0028 04da  ..%....(...i.(..
+000032a0: 02f0 baf9 6061 0420 70bd 02f0 bbf9 0020  ....`a. p...... 
+000032b0: 70bd feb5 0400 3f48 a030 007f c006 c00e  p.....?H.0......
+000032c0: 6061 02f0 75f9 6169 8003 0843 3949 6061  `a..u.ai...C9I`a
+000032d0: c97a 0029 00d0 0121 4906 0843 6061 3548  .z.)...!I..C`a5H
+000032e0: 2030 877a 7120 4006 0168 0025 0126 0191   0.zq @..h.%.&..
+000032f0: 3b49 3000 0968 a840 0842 13d0 7120 3b00  ;I0..h.@.B..q ;.
+00003300: 2900 4006 6a46 fff7 07f8 8028 0ad1 0199  ).@.jF.....(....
+00003310: 0098 8842 06d1 2a00 0832 3000 6169 9040  ...B..*..20.ai.@
+00003320: 0143 6161 6d1c 062d e2d3 224d 0121 4035  .Caam..-.."M.!@5
+00003330: e868 02f0 e2fb a061 a868 0121 02f0 ddfb  .h.....a.h.!....
+00003340: e061 2849 2034 0020 c201 5218 927b 2270  .a(I 4. ..R..{"p
+00003350: 641c 401c 1228 f7d3 1648 0189 2170 0089  d.@..(...H..!p..
+00003360: 000a 6070 1348 e030 017c a170 417c e170  ..`p.H.0.|.pA|.p
+00003370: 817c 2171 c07c 6071 2420 febd 0243 70b5  .|!q.|`q$ ...Cp.
+00003380: 0d00 1400 1000 01f0 9cee 0121 2a00 4904  ...........!*.I.
+00003390: 2043 0a43 0100 2120 4004 01f0 a2ec 70bd   C.C..! @.....p.
+000033a0: 00ff ff00 3809 4000 e800 4000 0020 0808  ....8.@...@.. ..
+000033b0: cd00 4000 007f 00e5 ffff 0000 780b 4000  ..@.........x.@.
+000033c0: 0001 ffff 2058 0000 5343 264d 502f 5370  .... X..SC&MP/Sp
+000033d0: 694e 4e61 6b65 7200 332e 302e 3100 0000  iNNaker.3.0.1...
+000033e0: e400 4000 2070 00e5 f8b5 8202 0f00 0101  ..@. p..........
+000033f0: 0323 9b06 890f 9843 4b1c 9b07 1e09 8b01  .#.....CK.......
+00003400: f649 0643 0020 5d18 a880 e880 0120 920f  .I.C. ]...... ..
+00003410: 0004 012a 00d0 0020 0024 e860 0120 a040  ...*... .$.`. .@
+00003420: 3842 11d0 2819 2030 007c 0028 0cd0 6000  8B..(. 0.|.(..`.
+00003430: 2818 018a a888 0322 401c a880 3000 9205  (......"@...0...
+00003440: 1040 3200 fff7 9aff 641c 102c e6d3 f8bd  .@2.....d..,....
+00003450: 0b00 e249 8201 5218 1189 d268 1b05 d218  ...I..R....h....
+00003460: 3f23 8006 9b06 c018 1218 0020 86e7 f3b5  ?#......... ....
+00003470: 81b0 0600 01f0 24ee 0028 31d1 3101 8c0f  ......$..(1.1...
+00003480: b102 3002 8d0f d549 800f 0028 29d1 3003  ..0....I...().0.
+00003490: 000b 002d 0bd1 a201 5218 d368 0504 2d0c  ...-....R..h..-.
+000034a0: 5b19 0125 2d04 2840 0343 d360 13e0 012d  [..%-.(@.C.`...-
+000034b0: 0cd1 a201 5318 da68 0126 1518 2d04 2d0c  ....S..h.&..-.-.
+000034c0: 3604 3040 0240 2a43 da60 04e0 a201 5218  6.0@.@*C.`....R.
+000034d0: d368 1818 d060 a001 4018 c188 491c c180  .h...`..@...I...
+000034e0: febd 002c 15d0 a201 5118 0298 0881 3101  ...,....Q.....1.
+000034f0: 0022 bb48 0909 d243 0523 02f0 43ff 0420  .".H...C.#..C.. 
+00003500: 031b c820 4343 b748 2a00 2100 02f0 3aff  ... CC.H*.!...:.
+00003510: febd 0124 0128 53d1 3006 000e 8446 3004  ...$.(S.0....F0.
+00003520: 000e 8646 3003 b04a 030f 0020 1268 0121  ...F0..J... .h.!
+00003530: 0ae0 ae4e 7746 765c 0124 3e40 6645 00d0  ...NwFv\.$>@fE..
+00003540: 0024 8c40 2043 491c 9142 f2d3 a84f 0024  .$.@ CI..B...O.$
+00003550: 022d 0fd1 0121 0ae0 0126 8e40 0642 05d0  .-...!...&.@.B..
+00003560: ce01 f619 b67b 9e42 00d1 641c 491c 9142  .....{.B..d.I..B
+00003570: f2d3 2ae0 002d 11d1 0121 0be0 0126 8e40  ..*..-...!...&.@
+00003580: 0642 06d0 ce01 f619 b67b 9e42 01d1 0124  .B.......{.B...$
+00003590: 2404 491c 9142 f1d3 641c 16e0 0124 2404  $.I..B..d....$$.
+000035a0: 0121 0ae0 0126 8e40 0642 05d0 ce01 f619  .!...&.@.B......
+000035b0: b67b 9e42 00d0 0024 491c 9142 f2d3 ebe7  .{.B...$I..B....
+000035c0: 0228 02d1 3000 fef7 e8f9 2805 0321 0019  .(..0.....(..!..
+000035d0: 8906 4218 0299 0020 fff7 d0fe febd 70b5  ..B.... ......p.
+000035e0: 0400 4169 8069 8422 0029 0ed1 8149 824b  ..Ai.i.".)...I.K
+000035f0: c989 1b68 9942 01d0 2282 24e0 0100 0120  ...h.B..".$.... 
+00003600: 7e4a 4004 01f0 6ceb 1de0 0129 10d1 e169  ~J@...l....)...i
+00003610: 0029 f1d0 0201 950f fff7 e6fe 7848 01f0  .)..........xH..
+00003620: 65fd 6e49 a801 4018 c068 6061 0420 b6e6  e.nI..@..h`a. ..
+00003630: 0229 e1d1 0521 3f22 0907 1202 4118 1002  .)...!?"....A...
+00003640: 0123 fef7 16ff 0020 a9e6 f8b5 0400 4069  .#..... ......@i
+00003650: 0306 0004 1b0e 050e 072b 02d9 8420 2082  .........+...  .
+00003660: 2de0 6448 634f 0026 2030 a037 01f0 2cee  -.dHcO.& 0.7..,.
+00003670: 0805 0d13 1923 2930 3a2e 2b02 e269 a169  .....#)0:.+..i.i
+00003680: c068 db1c 02f0 eafc 0fe0 a169 c068 0122  .h.........i.h."
+00003690: 02f0 4cfd 13e0 c068 0122 2900 02f0 90fd  ..L....h.").....
+000036a0: 13e0 a069 2900 01f0 41ff 6061 796a e800  ...i)...A.`ayj..
+000036b0: 401c 0e54 0ae0 e169 a069 01f0 cbff 0020  @..T...i.i..... 
+000036c0: f8bd a169 2800 02f0 1bf8 6061 0420 f8bd  ...i(.....`a. ..
+000036d0: c168 c968 6161 c068 0121 02f0 0efa a061  .h.haa.h.!.....a
+000036e0: 0820 f8bd a069 2900 0006 000e 02f0 5efc  . ...i).......^.
+000036f0: ebe7 10b5 4169 8269 8423 1229 01d9 0382  ....Ai.i.#.)....
+00003700: 13e0 d207 04d0 3b4a 6032 8a18 127d 02e0  ......;J`2...}..
+00003710: 3c4c 0a00 615c 002a f1d0 334c 2468 a242  <L..a\.*..3L$h.B
+00003720: edd2 0120 8840 00f0 28fe 0020 10bd 10b5  ... .@..(.. ....
+00003730: 8288 182a 01d2 8121 4ee0 038a 8022 0282  ...*...!N...."..
+00003740: 01f0 c2ed 2011 4914 1749 1a49 4949 4949  .... .I..I.IIIII
+00003750: 4949 4949 493a 2528 3731 4940 2b34 1d2e  IIIII:%(71I@+4..
+00003760: 223d 4349 4649 fff7 e4fc 10bd 02f0 00f9  "=CIFI..........
+00003770: 10bd 02f0 5ff9 10bd 02f0 f3f8 10bd 4069  ...._.........@i
+00003780: 02f0 38fb 0020 10bd fdf7 8cfd 10bd fff7  ..8.. ..........
+00003790: f3fc 10bd fff7 20fd 10bd fff7 05fc 10bd  ...... .........
+000037a0: fff7 49fc 10bd fff7 f5fb 10bd fff7 3ffd  ..I...........?.
+000037b0: 10bd fff7 43fd 10bd fff7 9bff 10bd fff7  ....C...........
+000037c0: 44ff 10bd fff7 0bff 10bd fff7 45fd 10bd  D...........E...
+000037d0: fff7 6ffd 10bd 8321 0182 d3e7 3804 4000  ..o....!....8.@.
+000037e0: e923 0000 5124 0000 0801 4000 5807 4000  .#..Q$....@.X.@.
+000037f0: 2070 00e5 207f 00e5 d400 4000 5555 ffff   p.. .....@.UU..
+00003800: 1027 0000 6c07 4000 0022 334b d243 10b5  .'..l.@.."3K.C..
+00003810: 07e0 0478 401c 5440 2406 a40d 1c59 120a  ...x@.T@$....Y..
+00003820: 6240 491e f5d2 d043 10bd 70b5 0500 0c00  b@I....C..p.....
+00003830: 01f0 42ec 2843 0122 0021 5207 4125 6d04  ..B.(C.".!R.A%m.
+00003840: 1368 002b fcda 8b04 2b43 1360 5460 9060  .h.+....+C.`T`.`
+00003850: 491c 0629 f4d3 2148 8078 01f0 47fc 70bd  I..)..!H.x..G.p.
+00003860: f8b5 1f49 8872 1e49 0020 4031 0870 1b21  ...I.r.I. @1.p.!
+00003870: 1c48 0904 fff7 d9ff 0025 1b48 2e04 a902  .H.......%.H....
+00003880: 3043 0091 fff7 d1ff 0024 2f02 3000 2102  0C.......$/.0.!.
+00003890: 0843 1649 8122 0843 3919 8900 d203 8918  .C.I.".C9.......
+000038a0: 0968 fff7 c2ff 641c ff2c efd9 1048 8121  .h....d..,...H.!
+000038b0: 0643 0098 c903 4018 0121 8902 fff7 a4ff  .C....@..!......
+000038c0: 0100 3000 fff7 b1ff 6d1c 1c2d d5d3 0948  ..0.....m..-...H
+000038d0: 0021 fff7 aaff f8bd 0054 0000 407f 00e5  .!.......T..@...
+000038e0: 8081 4000 0300 0001 03ff 0002 0300 0003  ..@.............
+000038f0: 0300 0004 0301 0005 0f00 2de9 fc03 9fe5  ..........-.....
+00003900: 0232 a0e3 0110 d0e5 0110 81e2 1f10 01e2  .2..............
+00003910: 0110 c0e5 8110 81e0 0111 80e0 0420 b1e5  ............. ..
+00003920: 0020 83e5 0208 12e3 0420 9115 0420 8315  . ....... ... ..
+00003930: 0810 91e5 0810 83e5 0210 d0e5 0110 41e2  ..............A.
+00003940: 0210 c0e5 0210 d0e5 1f04 a0e3 0000 51e3  ..............Q.
+00003950: 021b a003 1410 8005 3000 80e5 0f00 bde8  ........0.......
+00003960: 04f0 5ee2 0f50 2de9 0212 a0e3 1000 91e5  ..^..P-.........
+00003970: 1410 91e5 aa2c 81e2 ab20 92e2 b105 000b  .....,... ......
+00003980: 0f50 bde8 04f0 5ee2 0f50 2de9 0202 a0e3  .P....^..P-.....
+00003990: 0c30 90e5 1010 90e5 1420 90e5 8302 a0e1  .0....... ......
+000039a0: 0208 13e3 a00e a0e1 0130 02e2 0500 000a  .........0......
+000039b0: 0000 53e3 0100 000a 4afa fffb 0300 00ea  ..S.....J.......
+000039c0: 08fd fffb 0100 00ea 0000 53e3 9f05 001b  ..........S.....
+000039d0: 1f04 a0e3 3000 80e5 0f50 bde8 04f0 5ee2  ....0....P....^.
+000039e0: 0f50 2de9 0212 a0e3 1000 91e5 1410 91e5  .P-.............
+000039f0: 0127 a0e1 222f a0e1 0118 a0e1 0200 52e3  .'.."/........R.
+00003a00: 2118 a0e1 0100 001a 97fe fffb 0500 00ea  !...............
+00003a10: 0000 52e3 0100 001a 66f9 fffb 0100 00ea  ..R.....f.......
+00003a20: 0100 52e3 8b05 000b 1f04 a0e3 3000 80e5  ..R.........0...
+00003a30: 0f50 bde8 04f0 5ee2 ff50 2de9 2104 a0e3  .P....^..P-.!...
+00003a40: 0c00 80e5 b842 9fe5 d000 c4e1 1060 44e2  .....B.......`D.
+00003a50: 0100 90e2 0010 a1e2 f000 c4e1 b801 d6e1  ................
+00003a60: 0f5c 46e2 0140 80e2 fa0f 54e3 0c00 001a  .\F..@....T.....
+00003a70: 1c0f 95e5 0040 a0e3 0100 80e2 1c0f 85e5  .....@..........
+00003a80: 8002 9fe5 0230 a0e3 0420 a0e1 0410 a0e1  .....0... ......
+00003a90: 5306 00fa 0000 50e3 e720 a003 9a1f 8f02  S.....P.. ......
+00003aa0: d309 000b b841 c6e1 6862 9fe5 0000 96e5  .....A..hb......
+00003ab0: 0140 80e2 0a00 54e3 0900 001a 0040 a0e3  .@....T......@..
+00003ac0: 5402 9fe5 0130 a0e3 0420 a0e1 0410 a0e1  T....0... ......
+00003ad0: 4306 00fa 0000 50e3 f320 a003 8a1f 8f02  C.....P.. ......
+00003ae0: c309 000b 0020 a0e3 3002 9fe5 0130 a0e3  ..... ..0....0..
+00003af0: 0210 a0e1 3a06 00fa 0000 50e3 f720 a003  ....:.....P.. ..
+00003b00: 811f 8f02 ba09 000b 0040 86e5 0f1f d5e5  .........@......
+00003b10: 0000 51e3 0900 000a 200f 95e5 0100 80e2  ..Q..... .......
+00003b20: 200f 85e5 3001 a0e1 e114 a0e3 0020 91e5   ...0........ ..
+00003b30: 0300 00e2 c020 c2e3 0003 82e1 0000 81e5  ..... ..........
+00003b40: 1f04 a0e3 3000 80e5 ff50 bde8 04f0 5ee2  ....0....P....^.
+00003b50: ff5f 2de9 0060 a0e3 0170 a0e3 c001 9fe5  ._-..`...p......
+00003b60: c081 9fe5 ac51 9fe5 0010 90e5 ec2f 98e5  .....Q......./..
+00003b70: 0400 95e5 0100 80e2 0100 50e1 0400 85e5  ..........P.....
+00003b80: 0460 8525 0400 95e5 1700 12e1 f7ff ff0a  .`.%............
+00003b90: 0400 95e5 8043 88e0 3490 94e5 39a0 d4e5  .....C..4...9...
+00003ba0: 0100 a0e3 7105 00eb 0420 95e5 ec1f 98e5  ....q.... ......
+00003bb0: 1712 d1e1 ec1f 88e5 6c11 9f05 e224 a003  ........l....$..
+00003bc0: 0410 9105 1711 a001 0111 8102 7b15 8102  ............{...
+00003bd0: 0c10 8205 0110 a0e3 6d05 00eb 0100 5ae3  ........m.....Z.
+00003be0: 3960 c4e5 1000 001a 9e08 00fa 0040 b0e1  9`...........@..
+00003bf0: 0600 000a 0910 a0e1 0400 a0e1 8f05 00eb  ................
+00003c00: 0010 a0e3 0400 a0e1 0e01 00fb 0300 00ea  ................
+00003c10: 132e a0e3 f010 8fe2 0000 a0e3 7609 00fa  ............v...
+00003c20: 0900 a0e1 ca08 00fa 0300 00ea fc20 9fe5  ............. ..
+00003c30: d410 8fe2 0000 a0e3 6f09 00fa 1f04 a0e3  ........o.......
+00003c40: 3000 80e5 ff5f bde8 04f0 5ee2 0000 a0e3  0...._....^.....
+00003c50: 2114 a0e3 1040 2de9 2800 81e5 033c 4fe2  !....@-.(....<O.
+00003c60: 0120 a0e3 1810 a0e3 1000 a0e3 e708 00fa  . ..............
+00003c70: 0120 a0e3 bd3f 4fe2 1a10 a0e3 0200 a0e1  . ...?O.........
+00003c80: e208 00fa ab3f 4fe2 0120 a0e3 1910 a0e3  .....?O.. ......
+00003c90: 0200 a0e3 dd08 00fa ea3f 4fe2 0020 a0e3  .........?O.. ..
+00003ca0: 0b10 a0e3 0300 a0e3 d808 00fa 8030 9fe5  .............0..
+00003cb0: 0120 a0e3 0510 a0e3 0400 a0e3 d308 00fa  . ..............
+00003cc0: 7030 9fe5 0120 a0e3 1410 a0e3 0500 a0e3  p0... ..........
+00003cd0: ce08 00fa a93f 4fe2 0120 a0e3 0410 a0e3  .....?O.. ......
+00003ce0: 0600 a0e3 c908 00fa 1040 bde8 693f 4fe2  .........@..i?O.
+00003cf0: 0120 a0e3 1210 a0e3 0700 a0e3 c108 00ea  . ..............
+00003d00: a007 4000 107f 00e5 8136 0000 7363 616d  ..@......6..scam
+00003d10: 702d 6973 722e 6300 c400 4000 dd37 0000  p-isr.c...@..7..
+00003d20: 6d3a 0000 0801 4000 0070 00e5 780b 4000  m:....@..p..x.@.
+00003d30: 3701 0000 a052 0000 9001 0000 f848 0021  7....R.......H.!
+00003d40: 0b00 c289 1204 08d5 8289 002a 05d0 521e  ...........*..R.
+00003d50: 1204 120c 8281 00d1 c381 2030 491c 1029  .......... 0I..)
+00003d60: efd3 7047 ee49 0820 4201 5218 d289 002a  ..pG.I. B.R....*
+00003d70: 03d0 401c 0f28 f7d9 ff20 7047 ffb5 81b0  ..@..(... pG....
+00003d80: 8446 1d00 1700 fff7 edff 0600 ff28 17d0  .F...........(..
+00003d90: e349 7001 4418 0320 8003 2818 e081 0020  .Ip.D.. ..(.... 
+00003da0: 6781 a082 2100 6046 fdf7 2afb 0298 211d  g...!.`F..*...!.
+00003db0: fdf7 1ffb 002d 02d0 681e 0125 8540 a581  .....-..h..%.@..
+00003dc0: 3000 05b0 f0bd d749 0120 0870 7047 0170  0......I. .ppG.p
+00003dd0: 7047 827a 8189 c37a 8372 c272 c289 8281  pG.z...z.r.r....
+00003de0: c181 7047 70b5 0400 007a 0d00 0106 0fd5  ..pGp....z......
+00003df0: 4006 400e 2072 2000 fff7 ebff 002d 02d0  @.@. r ......-..
+00003e00: 0c20 2582 a080 0021 2000 00f0 1ef9 70bd  . %....! .....p.
+00003e10: 2000 02f0 19f8 70bd f8b5 0f00 c249 0600   .....p......I..
+00003e20: c001 4418 02f0 a8f8 0500 01d1 8a20 f8bd  ..D.......... ..
+00003e30: 3900 2800 01f0 04ea 0120 2563 2034 2076  9.(...... %c 4 v
+00003e40: b849 3439 895d 8840 b849 4018 7121 4906  .I49.].@.I@.q!I.
+00003e50: 8860 0020 0090 b648 0222 6946 01f0 60fa  .`. ...H."iF..`.
+00003e60: 0600 07d1 b34a b4a1 02f0 c8f9 2800 02f0  .....J......(...
+00003e70: 71f8 dbe7 7d21 7769 c900 3000 02f0 4afa  q...}!wi..0...J.
+00003e80: 207e 0028 03d0 6b46 1878 0028 f8d0 6b46   ~.(..kF.x.(..kF
+00003e90: 1878 0028 04d0 2800 02f0 5cf8 8620 f8bd  .x.(..(...\.. ..
+00003ea0: 3900 3000 02f0 04fa 8020 f8bd 9c4a f0b5  9.0...... ...J..
+00003eb0: 4001 8418 e089 8fb0 0204 68d5 06aa 0232  @.........h....2
+00003ec0: 0bab 0233 0293 8d88 c305 04d5 0f00 1037  ...3...........7
+00003ed0: 083d 0026 02e0 0f00 0837 0226 8005 01d5  .=.&.....7.&....
+00003ee0: a08a 02e0 8f48 2038 808a 6b46 0102 000a  .....H 8..kF....
+00003ef0: 0143 d985 ab19 0e93 1c33 1121 2000 fdf7  .C.......3.! ...
+00003f00: 90fa 0e9b 0833 1904 1802 090e 0843 6b46  .....3.......CkF
+00003f10: 5886 6089 0102 000a 0143 0020 1986 0200  X.`......C. ....
+00003f20: 9886 09a8 0821 0230 fdf7 faeb 0e9b 3100  .....!.0......1.
+00003f30: 1a18 0298 1932 0831 fdf7 f2eb 0200 2900  .....2.1......).
+00003f40: 3800 fdf7 eeeb c043 0102 0004 000e 0143  8......C.......C
+00003f50: 6b46 9986 03a9 201d 0191 fdf7 4afa 0199  kF.... .....J...
+00003f60: 7048 891d 1e38 fdf7 44fa 0820 6b46 1883  pH...8..D.. kF..
+00003f70: 3200 2b00 2a32 3900 03a8 fdf7 9bfa 0520  2.+.*29........ 
+00003f80: 01f0 b4f8 e089 4004 03d5 0020 e081 0fb0  ......@.... ....
+00003f90: f0bd 2069 401c 2061 f9e7 70b5 0400 007a  .. i@. a..p....z
+00003fa0: 4206 02d5 4022 9043 2072 674b 654e 1a69  B...@".C rgKeN.i
+00003fb0: a589 3240 b542 00d1 a281 e589 b542 00d1  ..2@.B.......B..
+00003fc0: e281 a289 e589 aa42 15d0 9d68 aa42 12d0  .......B...h.B..
+00003fd0: 8006 10d4 5869 0028 04d0 1000 01f0 6cfc  ....Xi.(......l.
+00003fe0: 0628 01d1 8721 2ce0 a089 2100 fdf7 acfd  .(...!,...!.....
+00003ff0: 17e0 0100 25e0 a27a ff2a 04d1 607a 2100  ....%..z.*..`z!.
+00004000: fff7 54ff 0fe0 db6b d006 c00e 9842 01d3  ..T....k.....B..
+00004010: 8821 16e0 4d4b 1b68 8342 08d0 2100 fff7  .!..MK.h.B..!...
+00004020: fbfe 8028 e5d1 2000 01f0 0eff 70bd 5009  ...(.. .....p.P.
+00004030: 06d1 2000 fff7 7bfb 0c30 0021 a080 00e0  .. ...{..0.!....
+00004040: 8521 2000 fff7 cefe 70bd 0a00 0100 4048  .! .....p.....@H
+00004050: 0023 10b5 01f0 c6f9 10bd f3b5 85b0 0598  .#..............
+00004060: 3049 0700 0e37 1839 1e30 fdf7 cef9 0028  0I...7.9.0.....(
+00004070: 72d0 3878 0599 0007 800e 0e18 0e36 7088  r.8x.........6p.
+00004080: 0106 090c 000a 0143 3088 0206 120c 000a  .......C0.......
+00004090: 0243 0392 b088 0206 150c 000a 0543 2148  .C...........C!H
+000040a0: 2038 808a 8842 5dd1 ff20 0a3d 1930 8542   8...B].. .=.0.B
+000040b0: 6ddc 01f0 d9fe 0400 02d1 ff22 4c32 6fe0  m.........."L2o.
+000040c0: 3100 2000 2a00 0a31 0830 01f0 c2e8 1e48  1. .*..1.0.....H
+000040d0: a580 8068 e081 3800 0c30 267a 657a 0700  ...h..8..0&zez..
+000040e0: 01a9 fdf7 8df9 ff2d 0bd1 3006 09d5 1648  .......-..0....H
+000040f0: 0599 c369 039a 891d 3800 fff7 3ffe 0540  ...i....8...?..@
+00004100: 6572 1448 0061 3006 07d5 102d 25d2 0448  er.H.a0....-%..H
+00004110: 6901 0818 c089 0028 1fd0 0199 2000 71e0  i......(.... .q.
+00004120: 3809 4000 a007 4000 0070 00e5 0000 c05e  8.@...@..p.....^
+00004130: cf2d 0000 4902 0000 7363 616d 702d 332e  .-..I...scamp-3.
+00004140: 6300 0000 ffff 0000 cc00 4000 780b 4000  c.........@.x.@.
+00004150: 9b2f 0000 00c0 00e4 19e0 2000 01f0 74fe  ./........ ...t.
+00004160: 07b0 f0bd 083d ff20 1130 8542 0295 0edc  .....=. .0.B....
+00004170: 0024 6001 ff4a 8018 c289 002a 02d0 808a  .$`..J.....*....
+00004180: 8842 02d0 641c 082c f3d3 082c 02d1 fa48  .B..d..,...,...H
+00004190: 0061 e5e7 01f0 68fe 0500 06d1 ff22 8432  .a....h......".2
+000041a0: f649 0020 02f0 2af8 f1e7 f24a 6001 8018  .I. ..*....J`...
+000041b0: 0399 0490 4181 3800 0499 0c30 fdf7 20f9  ....A.8....0.. .
+000041c0: 0498 011d 0598 801d fdf7 13f9 3100 2800  ............1.(.
+000041d0: 029a 0831 1030 00f0 d0ed e748 0061 0720  ...1.0.....H.a. 
+000041e0: 2872 e748 6c72 8068 e881 ff20 e872 0298  (r.Hlr.h... .r..
+000041f0: 0021 0830 a880 0498 c08a a881 0498 007e  .!.0...........~
+00004200: a872 2800 fff7 21ff aae7 10b5 da4c 6068  .r(...!......L`h
+00004210: 4006 800e 02d1 1020 2062 10bd e06a d949  @......  b...j.I
+00004220: 8006 000e 4018 0068 4105 606a 490d d64a  ....@..hA.`jI..J
+00004230: 0005 000d 8018 027b 437b 1202 d218 0123  .......{C{.....#
+00004240: db02 9a42 0ad1 c27d 112a 02d1 fff7 05ff  ...B...}.*......
+00004250: dde7 012a 09d1 fdf7 def9 d8e7 cb4b 9a42  ...*.........K.B
+00004260: 03d1 1022 fdf7 8ef9 d1e7 2461 cfe7 c84a  ..."......$a...J
+00004270: c101 f8b5 8c18 0221 2500 2035 2976 c549  .......!%. 5)v.I
+00004280: 095c 0120 8840 c449 4018 7121 4906 8860  .\. .@.I@.q!I..`
+00004290: 0020 0090 c148 0222 6946 01f0 41f8 0600  . ...H."iF..A...
+000042a0: 04d1 bf4a b549 01f0 a9ff 18e0 7d21 7769  ...J.I......}!wi
+000042b0: c900 3000 02f0 2ef8 287e 0028 03d0 6b46  ..0.....(~.(..kF
+000042c0: 1878 0028 f8d0 6b46 1878 0028 01d0 0020  .x.(..kF.x.(... 
+000042d0: f8bd 3900 3000 01f0 ebff 206b a062 0120  ..9.0..... k.b. 
+000042e0: f8bd f8b5 0400 0020 ae4a ff25 8118 401c  ....... .J.%..@.
+000042f0: 1428 0d75 fad3 ac49 0020 a318 a94e 0860  .(.u...I. ...N.`
+00004300: 1875 2036 a248 3472 c861 0120 0021 7127  .u 6.H4r.a. .!q'
+00004310: 7f06 a142 0ad0 3a69 0123 8b40 1a42 05d0  ...B..:i.#.@.B..
+00004320: a04a 8a18 1075 8219 401c 1172 491c 1229  .J...u..@..rI..)
+00004330: efd3 9349 c863 3077 02e0 8119 401c 0d72  ...I.c0w....@..r
+00004340: 1428 fad3 00f0 00ef 0500 3869 0121 a140  .(........8i.!.@
+00004350: 0842 02d1 0220 01f0 4dfd 3969 9348 8843  .B... ..M.9i.H.C
+00004360: 8d49 4018 7860 2800 00f0 f6ee 8d49 8948  .I@.x`(......I.H
+00004370: 1422 2831 00f0 6cef f8bd 7121 4906 10b5  ."(1..l...q!I...
+00004380: 4861 8948 4068 fff7 acff fdf7 6efa 7c48  Ha.H@h......n.|H
+00004390: 7f49 c06b 8022 c001 4018 0021 00f0 82ef  .I.k."..@..!....
+000043a0: 10bd f0b5 824e 0168 0660 8c46 0021 0127  .....N.h.`.F.!.'
+000043b0: 3a00 8a40 491c 9200 8358 8150 0468 8558  :..@I....X.P.h.X
+000043c0: 8350 8d42 01d1 b442 f2d0 6246 0260 0129  .P.B...B..bF.`.)
+000043d0: 01d1 0020 f0bd 491c 3800 8840 f0bd 10b5  ... ..I.8..@....
+000043e0: 7448 cab0 0690 7448 0790 01a8 fcf7 5aff  tH....tH......Z.
+000043f0: 724c ff22 0132 2000 06a9 00f0 2aef 2068  rL.".2 .....*. h
+00004400: 4028 02d2 6748 4030 8463 4ab0 10bd 6548  @(..gH@0.cJ...eH
+00004410: f8b5 2022 a038 6a49 00f0 1aef 6149 5d48  .. ".8jI....aI]H
+00004420: 2022 6031 1430 00f0 14ef 6648 4022 0021   "`1.0....fH@".!
+00004430: 00f0 38ef 574c 1434 2088 0004 01d5 fff7  ..8.WL.4 .......
+00004440: ceff 584e 803e b07a 0028 05d1 2088 0104  ..XN.>.z.(.. ...
+00004450: 02d5 0006 000f b072 524d 5b4f 514c 4035  .......rRM[OQL@5
+00004460: 5a48 ef63 403c 6860 a168 8900 4018 4849  ZH.c@<h`.h..@.HI
+00004470: 01f0 34fb 0922 a060 4548 1202 0021 00f0  ..4..".`EH...!..
+00004480: 12ef 4348 4249 e860 0720 2031 8873 4048  ..CHBI.`.  1.s@H
+00004490: 4030 c761 f269 4260 4348 4068 4873 3c48  @0.a.iB`CH@hHs<H
+000044a0: 4b49 4830 00f0 beee 6178 ff20 2530 4143  KIH0....ax. %0AC
+000044b0: 0022 a068 1300 01f0 d1fd a862 ff22 a062  .".h.......b.".b
+000044c0: 6178 2532 01f0 44fa a078 0028 06d1 3548  ax%2..D..x.(..5H
+000044d0: 2030 407f 0028 01d1 0120 2070 f8bd 3148   0@..(...  p..1H
+000044e0: f8b5 6038 c088 00f0 d3ff 0327 7f07 3800  ..`8.......'..8.
+000044f0: fff7 57ff 2b4d 0100 403d 6e69 6f61 a869  ..W.+M..@=nioa.i
+00004500: 4822 5043 274c 3818 4034 2060 ea68 891b  H"PC'L8.@4 `.h..
+00004510: 9200 cf19 8018 3900 01f0 e0fa e860 0125  ......9......`.%
+00004520: ad04 b108 7819 8900 0918 491b a760 01f0  ....x.....I..`..
+00004530: d5fa 0022 2900 1300 2061 01f0 8ffd 2549  ...")... a....%I
+00004540: 2a00 a061 00f0 aeee 0022 2349 2069 1300  *..a....."#I i..
+00004550: 01f0 84fd 0022 6061 2069 2900 1300 01f0  ....."`a i).....
+00004560: 7dfd 2a00 0021 e061 00f0 9cee 0022 ed11  }.*..!.a....."..
+00004570: 2900 33e0 3809 4000 00c0 00e4 3831 0000  ).3.8.@.....81..
+00004580: cc00 4000 0080 00e4 0040 00e4 0608 0000  ..@......@......
+00004590: 0070 00e5 6c07 4000 0000 c05e cf2d 0000  .p..l.@....^.-..
+000045a0: 1d02 0000 807f 00e5 780b 4000 ffff 0300  ........x.@.....
+000045b0: aa55 00ff 2000 0001 0001 0003 0079 00e5  .U.. ........y..
+000045c0: 0058 0000 c07f 00f5 0100 0300 0001 00e5  .X..............
+000045d0: 2458 0000 ffff 0080 1040 0000 2069 1300  $X.......@.. i..
+000045e0: 01f0 3cfd 2a00 0021 6062 00f0 5cee f8bd  ..<.*..!`b..\...
+000045f0: ff48 0022 0121 10b5 0069 8902 1300 01f0  .H.".!...i......
+00004600: 2dfd fb4c c03c e16b 0029 0dd1 a522 cb07  -..L.<.k.)..."..
+00004610: 02d0 8b00 c358 02e0 8b00 c358 db43 5a40  .....X.....X.CZ@
+00004620: 491c ff29 f3d9 e263 e06b 00f0 f5fd 10bd  I..)...c.k......
+00004630: f8b5 0021 0c00 ef48 0b00 456a ee4e 0120  ...!...H..Ej.N. 
+00004640: c201 9219 2032 977b 002f 00d0 491c d77b  .... 2.{./..I..{
+00004650: 002f 06d0 527b 641c 0127 9740 2f42 00d1  ./..R{d..'.@/B..
+00004660: 5b1c 401c 1228 ebd3 1802 c01a 00f0 deec  [.@..(..........
+00004670: 002c 02d0 0028 00d1 0120 e049 0870 f8bd  .,...(... .I.p..
+00004680: df48 10b5 0088 c007 07d0 0120 fcf7 d6fd  .H......... ....
+00004690: d749 4007 c00f c039 c872 10bd f1b5 0027  .I@....9.r.....'
+000046a0: d64c d549 6068 d74d c201 5118 2031 897b  .L.I`h.M..Q. 1.{
+000046b0: 0126 0429 04d3 fff7 dafd 0028 6068 08d0  .&.).......(`h..
+000046c0: 2f54 6068 401c 6060 e16b 8842 00d3 6660  /T`h@.``.k.B..f`
+000046d0: f8bd 295c 491c 0906 090e 2954 009a 9142  ..)\I.....)T...B
+000046e0: efd1 c749 1439 095c 3000 8840 0021 fdf7  ...I.9.\0..@.!..
+000046f0: 45f8 6068 c101 c048 0818 0321 2030 8173  E.`h...H...! 0.s
+00004700: dfe7 70b5 0025 bd4c 6570 b948 a038 4573  ..p..%.Lep.H.8Es
+00004710: b748 8038 0078 0028 02d0 e564 2565 02e0  .H.8.x.(...d%e..
+00004720: b948 e064 2065 6565 a565 e565 2566 b048  .H.d eee.e.e%f.H
+00004730: 0126 0022 f603 0069 3100 1300 01f0 8efc  .&."...i1.......
+00004740: 3200 0021 2062 00f0 aeed 6564 a564 70bd  2..! b....ed.dp.
+00004750: f0b5 85b0 4026 a949 0869 c208 4007 400f  ....@&.I.i..@.@.
+00004760: 0292 4200 8018 0190 a148 a038 877a 0024  ..B......H.8.z.$
+00004770: 0120 a040 a149 0490 8969 0842 22d0 0298  . .@.I...i.B"...
+00004780: a249 0225 8000 4018 0390 0398 3b00 2100  .I.%..@.....;.!.
+00004790: 6a46 fdf7 c1fd 8028 07d0 6d1e f5d1 9c4a  jF.....(..m....J
+000047a0: 9c49 0020 01f0 2afd 0ce0 0621 e01c 00f0  .I. ..*....!....
+000047b0: 3eec 019a 0098 d040 4007 400f 8142 01d1  >......@@.@..B..
+000047c0: 0498 0643 641c 062c d2d3 0022 9249 3300  ...Cd..,...".I3.
+000047d0: d243 0020 01f0 32f8 05b0 f0bd f8b5 874c  .C. ..2........L
+000047e0: 6078 0126 0025 0028 5dd0 0128 74d0 0228  `x.&.%.(]..(t..(
+000047f0: 73d0 0328 41d1 e068 070a 0006 000e 4743  s..(A..h......GC
+00004800: 6420 4743 e06a 0028 13d1 8449 a068 0968  d GC.j.(...I.h.h
+00004810: 8000 0d50 a068 0721 01f0 76f8 00f0 ceec  ...P.h.!..v.....
+00004820: 3900 00f0 04ec 4b1c 0022 7d48 1100 01f0  9.....K.."}H....
+00004830: a9fd 7c49 3800 00f0 faeb e16a 801c 4a1c  ..|I8......j..J.
+00004840: 8842 e262 19d8 6a4f e562 c03f 387b 411e  .B.b..jO.b.?8{A.
+00004850: 0028 3973 11d1 ff20 6070 fdf7 e4fc fff7  .(9s... `p......
+00004860: 77ff 6748 6661 be71 0088 c007 05d0 0120  w.gHfa.q....... 
+00004870: fcf7 e4fc 4007 c00f f872 6178 5c48 a038  ....@....rax\H.8
+00004880: 4173 6078 ff28 7ed1 a068 010a 0818 8100  As`x.(~..h......
+00004890: 4018 0106 206b 090e 8842 75d1 2178 8029  @... k...Bu.!x.)
+000048a0: 73d2 ff21 95e0 0021 0800 fdf7 55fe 606c  s..!...!....U.`l
+000048b0: 411c 6164 4e49 a039 097b 8842 ddd9 6670  A.adNI.9.{.B..fp
+000048c0: e06c 0028 01da e06c 00e0 0020 6065 206d  .l.(...l... `e m
+000048d0: 0028 03da 206d 02e0 11e0 5de0 0020 e065  .(.. m....].. .e
+000048e0: e06c 0028 01dd e06c 00e0 0020 a065 206d  .l.(...l... .e m
+000048f0: 0028 01dd 206d 00e0 0020 2066 bde7 0021  .(.. m...  f...!
+00004900: 0800 fdf7 67fe a06c 411c a164 384f a03f  ....g..lA..d8O.?
+00004910: 397b 8842 b1d9 e16c 3b48 8142 02d0 216d  9{.B...l;H.B..!m
+00004920: 8142 02d1 4048 fff7 28fd e06c 616d 401a  .B..@H..(..lam@.
+00004930: 216d 0002 e26d 2e4e 891a 0843 c03e a060  !m...m.N...C.>.`
+00004940: 3080 a16d 626d 891a 226e 491c 0902 e36d  0..mbm.."nI....m
+00004950: d21a 521c 1143 e160 7180 616d e26d 4942  ..R..C.`q.am.mIB
+00004960: 0902 5242 1143 2161 f981 2149 2031 4a88  ..RB.C!a..!I 1J.
+00004970: 521c 4a80 00f0 50fc a068 0721 0906 4018  R.J...P..h.!..@.
+00004980: 0121 4907 02e0 2be0 25e0 21e0 8861 fdf7  .!I...+.%.!..a..
+00004990: e7fb 0220 a562 19e0 a06a 401c 0128 a062  ... .b...j@..(.b
+000049a0: 10d1 1348 866b 002e a8d0 80ce 07e0 0021  ...H.k.........!
+000049b0: 3268 0800 fef7 75f9 01ce fdf7 88fd 7f1e  2h....u.........
+000049c0: f5d2 5ae7 0328 99d3 0320 e562 6070 54e7  ..Z..(... .b`pT.
+000049d0: 0021 4900 6162 401c ff28 2063 00d9 2563  .!I.ab@..( c..%c
+000049e0: 00f0 eceb 0f49 491e 00f0 20eb 4b1c 1de0  .....II... .K...
+000049f0: c07f 00e5 4000 00e2 0070 00e5 cc00 4000  ....@....p....@.
+00004a00: 8007 4000 2409 4000 00fc ffff 0000 01e1  ..@.$.@.........
+00004a10: 7104 0000 3831 0000 5555 ffff 3000 4000  q...81..UU..0.@.
+00004a20: 2516 0000 1027 0000 ffff 0300 0022 a148  %....'.......".H
+00004a30: 1100 01f0 a7fc fff7 81f9 9f48 c078 0028  ...........H.x.(
+00004a40: 01d0 fff7 2bfe 9c4a 403a 508b 0028 0cd0  ....+..J@:P..(..
+00004a50: 216c 491c 8142 2164 07d3 2564 116a 3f22  !lI..B!d..%d.j?"
+00004a60: 9648 1202 0023 fdf7 04fd f8bd 70b5 944c  .H...#......p..L
+00004a70: 6078 ff28 29d3 9048 0025 2038 c07a 0128  `x.()..H.% 8.z.(
+00004a80: 24d1 2078 616a 4000 8142 02d2 606a 401c  $. xaj@..B..`j@.
+00004a90: 04e0 616a 8142 02d9 606a 401e 6062 606a  ..aj.B..`j@.`b`j
+00004aa0: 616a 4009 0029 02d0 0028 00d1 0120 616b  aj@..)...(... ak
+00004ab0: 8142 01d3 0220 00e0 0320 01f0 9bf9 606b  .B... ... ....`k
+00004ac0: 401c 1028 6063 00d3 6563 70bd 0228 fcd3  @..(`c..ecp..(..
+00004ad0: a16b 4a1c a263 0a22 5043 8142 f5d9 0120  .kJ..c."PC.B... 
+00004ae0: a563 01f0 87f9 70bd feb5 0a21 7548 764c  .c....p....!uHvL
+00004af0: 0186 0020 2062 0220 00f0 f8fa 6e48 2038  ...  b. ....nH 8
+00004b00: 8188 c088 4d00 4600 2900 6846 00f0 f8ea  ....M.F.).hF....
+00004b10: 2800 00f0 c3f8 6d4f 0099 c019 4018 2061  (.....mO....@. a
+00004b20: 3100 6846 00f0 ecea 3000 00f0 b7f8 0099  1.hF....0.......
+00004b30: c019 4018 6061 5020 00f0 d8fa 5e48 ea03  ..@.`aP ....^H..
+00004b40: 4038 807b 5f4b 0109 491e 401e 8907 8007  @8.{_K..I.@.....
+00004b50: 090a 400b 0818 5e49 120c 4018 1a86 2062  ..@...^I..@... b
+00004b60: febd 70b5 5b4d 2888 c007 2ed0 2c00 a81c  ..p.[M(.....,...
+00004b70: fcf7 28fc 5048 2900 0422 0831 b030 00f0  ..(.PH)..".1.0..
+00004b80: 68eb 2088 4007 01d5 fcf7 1efb 2888 0007  h. .@.......(...
+00004b90: 09d5 ff21 e231 0420 fcf7 3cfb 0921 4902  ...!.1. ..<..!I.
+00004ba0: 0020 fcf7 37fb 444c 403c 0be0 0120 fcf7  . ..7.DL@<... ..
+00004bb0: 45fb 4007 c00f e072 e07a 0028 05d1 0120  E.@....r.z.(... 
+00004bc0: 00f0 1afc 2888 8007 f0d4 70bd 3e49 0120  ....(.....p.>I. 
+00004bd0: 70b5 c006 c860 7124 6406 a06b 4d02 2843  p....`q$d..kM.(C
+00004be0: a063 0120 00f0 82fa a06b a843 a063 70bd  .c. .....k.C.cp.
+00004bf0: 1021 4020 0176 0021 8076 0177 417f 4908  .!@ .v.!.v.wA.I.
+00004c00: 4900 4177 7047 70b5 a020 2e4c 2086 fff7  I.AwpGp.. .L ...
+00004c10: ddff 3249 3048 0860 0020 e321 0906 8860  ..2I0H.`. .!...`
+00004c20: 7120 4006 816b 0125 2943 8163 6068 fff7  q @..k.%)C.c`h..
+00004c30: 58fb fff7 ecfb 01f0 bdf8 fff7 55ff fff7  X...........U...
+00004c40: 4efc fff7 d5fc 6068 00f0 7afd 1a4e b078  N.....`h..z..N.x
+00004c50: 0028 04d0 1848 4038 807a fef7 01fe fcf7  .(...H@8.z......
+00004c60: 04fe 208e 7d21 c900 4843 e222 2121 0906  .. .}!..HC."!!..
+00004c70: 8a60 0860 1748 2030 0570 fdf7 59fa fff7  .`.`.H 0.p..Y...
+00004c80: 40fd fef7 e4ef b078 0028 01d0 fff7 69ff  @......x.(....i.
+00004c90: 0120 00f0 b1fb 00f0 d0ea f9e7 0021 3228  . ...........!2(
+00004ca0: 00d3 0121 6428 00d3 0221 c828 00d3 0321  ...!d(...!.(...!
+00004cb0: 0804 7047 3136 0000 407f 00e5 0000 3e02  ..pG16..@.....>.
+00004cc0: cc00 4000 780b 4000 4000 00e2 0001 0400  ..@.x.@.@.......
+00004cd0: a588 1080 8007 4000 51e5 cc1a 000c 00e3  ......@.Q.......
+00004ce0: f041 2de9 0150 a0e1 0070 a0e1 8040 9fe5  .A-..P...p...@..
+00004cf0: 0260 a0e1 1901 00eb 0210 d4e5 2000 51e3  .`.......... .Q.
+00004d00: 0200 003a 1301 00eb 0000 a0e3 f081 bde8  ...:............
+00004d10: 0210 d4e5 0000 51e3 021b a003 1f24 a003  ......Q......$..
+00004d20: 1010 8205 0210 d4e5 0110 81e2 0210 c4e5  ................
+00004d30: 0210 d4e5 0320 d4e5 0200 51e1 0210 d485  ..... ....Q.....
+00004d40: 0310 c485 0030 d4e5 8310 83e0 0111 84e0  .....0..........
+00004d50: 0470 a1e5 6000 81e9 0010 d4e5 0110 81e2  .p..`...........
+00004d60: 1f10 01e2 0010 c4e5 fa00 00eb 0100 a0e3  ................
+00004d70: f081 bde8 a007 4000 0300 52e3 2a00 009a  ......@...R.*...
+00004d80: 03c0 10e2 0800 000a 0130 d1e4 0200 5ce3  .........0....\.
+00004d90: 0c20 82e0 01c0 d194 0130 c0e4 0130 d134  . .......0...0.4
+00004da0: 01c0 c094 0420 42e2 0130 c034 0330 11e2  ..... B..0.4.0..
+00004db0: 8400 000a 0420 52e2 1b00 003a 03c0 31e7  ..... R....:..1.
+00004dc0: 0200 53e3 0800 000a 0f00 008a 2c34 a0e1  ..S.........,4..
+00004dd0: 04c0 b1e5 0420 52e2 0c3c 83e1 0430 80e4  ..... R..<...0..
+00004de0: f9ff ff2a 0110 81e2 0f00 00ea 2c38 a0e1  ...*........,8..
+00004df0: 04c0 b1e5 0420 52e2 0c38 83e1 0430 80e4  ..... R..8...0..
+00004e00: f9ff ff2a 0210 81e2 0700 00ea 2c3c a0e1  ...*........,<..
+00004e10: 04c0 b1e5 0420 52e2 0c34 83e1 0430 80e4  ..... R..4...0..
+00004e20: f9ff ff2a 0310 81e2 0000 a0e1 822f b0e1  ...*........./..
+00004e30: 0130 d124 01c0 d124 0120 d144 0130 c024  .0.$...$. .D.0.$
+00004e40: 01c0 c024 0120 c044 1eff 2fe1 0130 90e1  ...$. .D../..0..
+00004e50: 2100 004a 0020 b0e3 a030 71e0 1a00 003a  !..J. ...0q....:
+00004e60: 2032 71e0 0f00 003a 2034 71e0 0100 003a   2q....: 4q....:
+00004e70: 00c0 a0e3 2000 00ea a033 71e0 8103 4020  .... ....3q...@ 
+00004e80: 0220 b2e0 2033 71e0 0103 4020 0220 b2e0  . .. 3q...@ . ..
+00004e90: a032 71e0 8102 4020 0220 b2e0 2032 71e0  .2q...@ . .. 2q.
+00004ea0: 0102 4020 0220 b2e0 a031 71e0 8101 4020  ..@ . ...1q...@ 
+00004eb0: 0220 b2e0 2031 71e0 0101 4020 0220 b2e0  . .. 1q...@ . ..
+00004ec0: a030 71e0 8100 4020 0220 b2e0 0110 50e0  .0q...@ . ....P.
+00004ed0: 0010 a031 0200 a2e0 1eff 2fe1 0221 11e2  ...1....../..!..
+00004ee0: 0010 6142 40c0 32e0 0000 6022 2032 71e0  ..aB@.2...`" 2q.
+00004ef0: 1d00 003a 2034 71e0 0f00 003a 0113 a0e1  ...: 4q....:....
+00004f00: 2034 71e0 3f23 82e3 0b00 003a 0113 a0e1   4q.?#.....:....
+00004f10: 2034 71e0 3f26 82e3 0700 003a 0113 a0e1   4q.?&.....:....
+00004f20: 2034 71e0 3f29 82e3 0113 a021 3f2c 8223   4q.?).....!?,.#
+00004f30: 0030 71e2 1d00 002a 2113 a021 a033 71e0  .0q....*!..!.3q.
+00004f40: 8103 4020 0220 b2e0 2033 71e0 0103 4020  ..@ . .. 3q...@ 
+00004f50: 0220 b2e0 a032 71e0 8102 4020 0220 b2e0  . ...2q...@ . ..
+00004f60: 2032 71e0 0102 4020 0220 b2e0 a031 71e0   2q...@ . ...1q.
+00004f70: 8101 4020 0220 b2e0 2031 71e0 0101 4020  ..@ . .. 1q...@ 
+00004f80: 0220 b2e0 ebff ff2a a030 71e0 8100 4020  . .....*.0q...@ 
+00004f90: 0220 b2e0 0110 50e0 0010 a031 0200 a2e0  . ....P....1....
+00004fa0: cccf b0e1 0000 6042 0010 6122 1eff 2fe1  ......`B..a"../.
+00004fb0: cccf b0e1 0000 6042 0140 2de9 0000 b0e3  ......`B.@-.....
+00004fc0: 0000 a0e1 0280 bde8 1040 2de9 2020 52e2  .........@-.  R.
+00004fd0: 0500 003a 1850 b1e8 2020 52e2 1850 a0e8  ...:.P..  R..P..
+00004fe0: 1850 b1e8 1850 a0e8 f9ff ff2a 02ce b0e1  .P...P.....*....
+00004ff0: 1850 b128 1850 a028 1800 b148 1800 a048  .P.(.P.(...H...H
+00005000: 1040 bde8 02cf b0e1 0430 9124 0430 8024  .@.......0.$.0.$
+00005010: 1eff 2f01 822f b0e1 b230 d120 0120 d144  ../../...0. . .D
+00005020: b230 c020 0120 c044 1eff 2fe1 0020 b0e3  .0. . .D../.. ..
+00005030: 2032 71e0 9bff ff3a 2034 71e0 8dff ff3a   2q....: 4q....:
+00005040: 00c0 a0e3 acff ffea 04f0 1fe5 9b09 0000  ................
+00005050: 04f0 1fe5 0113 0000 04f0 1fe5 bb10 0000  ................
+00005060: f2b5 0549 05a6 4027 3cce 3cc1 103f fbd1  ...I..@'<.<..?..
+00005070: 041c 3f39 0847 0000 c07f 0000 0fcc 0128  ..?9.G.........(
+00005080: 08d0 0228 04d0 0328 0bd0 0428 11d0 f2bd  ...(...(...(....
+00005090: 1219 103a e1ca e1c1 e1ca e1c1 203b f9d8  ...:........ ;..
+000050a0: ece7 1d1c 1e1c 1f1c e8c1 e8c1 203a fbd8  ............ :..
+000050b0: e4e7 0098 8847 e1e7 0100 90e0 0100 8022  .....G........."
+000050c0: 0008 90e0 0108 8022 ff0c c0e3 0004 90e0  ......."........
+000050d0: 0104 8022 ff08 c0e3 0002 90e0 0102 8022  ..."..........."
+000050e0: 0f02 00e2 0f02 20e2 1eff 2fe1 0349 0988  ...... .../..I..
+000050f0: 4143 8808 0138 fdd2 7047 0000 a80b 4000  AC...8..pG....@.
+00005100: 0a20 41e2 2111 41e0 2112 81e0 2114 81e0  . A.!.A.!...!...
+00005110: 2118 81e0 a111 a0e1 0131 81e0 8320 52e0  !........1... R.
+00005120: 0110 8152 0a20 8242 0600 80e8 1eff 2fe1  ...R. .B....../.
+00005130: 0030 0fe1 01f0 21e1 00d0 a0e1 03f0 2fe1  .0....!......./.
+00005140: 0201 40e0 1eff 2fe1 0000 0fe1 c010 80e3  ..@.../.........
+00005150: 01f0 21e1 1eff 2fe1 00f0 2fe1 1eff 2fe1  ..!.../.../.../.
+00005160: 0000 0fe1 8010 80e3 01f0 21e1 1eff 2fe1  ..........!.../.
+00005170: e2c4 a0e3 00c1 8ce0 0000 0fe1 c010 80e3  ................
+00005180: 01f0 21e1 0011 9ce5 0201 11e3 fcff ff1a  ..!.............
+00005190: 1eff 2fe1 e2c4 a0e3 0111 8ce0 8011 91e5  ../.............
+000051a0: 00f0 21e1 1eff 2fe1 0120 52e2 0130 d124  ..!.../.. R..0.$
+000051b0: 0130 c024 fbff ff2a 1eff 2fe1 1c30 9fe5  .0.$...*../..0..
+000051c0: 0300 93e8 a100 11e1 6020 b0e1 0110 a1e0  ........` ......
+000051d0: 0026 22e0 220a 22e0 0300 83e8 1eff 2fe1  .&"."."......./.
+000051e0: 800b 4000 0f50 2de9 0400 4ee2 00c0 4fe1  ..@..P-...N...O.
+000051f0: 1ff0 21e3 0050 2de9 9502 00fa 0050 bde8  ..!..P-......P..
+00005200: 92f0 21e3 0cf0 6fe1 2f04 a0e3 3000 80e5  ..!...o./...0...
+00005210: 0f50 bde8 04f0 5ee2 014a 0021 03c2 7047  .P....^..J.!..pG
+00005220: 800b 4000 0120 d1e4 0000 52e3 0120 c0e4  ..@.. ....R.. ..
+00005230: fbff ff1a 1eff 2fe1 900f 07ee 1eff 2fe1  ....../......./.
+00005240: 0400 80e2 0410 81e2 b020 d1e1 0420 82e2  ......... ... ..
+00005250: 0300 12e3 0320 c213 0420 8212 1040 2de9  ..... ... ...@-.
+00005260: 2020 52e2 0500 003a 1850 b1e8 1850 a0e8    R....:.P...P..
+00005270: 1850 b1e8 1850 a0e8 2020 52e2 f9ff ff2a  .P...P..  R....*
+00005280: 02ce b0e1 1850 b128 1850 a028 1800 b148  .....P.(.P.(...H
+00005290: 1800 a048 02cf b0e1 0430 9124 0430 8024  ...H.....0.$.0.$
+000052a0: 1080 bde8 0130 a0e1 1020 52e2 0a00 a028  .....0... R....(
+000052b0: 0a00 a028 fbff ff2a 822e b0e1 0a00 a028  ...(...*.......(
+000052c0: 0200 a048 1eff 2fe1 01c0 5ee5 0c00 53e1  ...H../...^...S.
+000052d0: 0330 de37 0c30 de27 83c0 8ee0 1cff 2fe1  .0.7.0.'....../.
+000052e0: 70b5 0600 1821 00f0 27fb 0c4d 0400 0ed0  p....!..'..M....
+000052f0: 1822 3100 2000 00f0 2bfb 0600 fff7 24ef  ."1. ...+.....$.
+00005300: 2968 3160 2c60 fff7 28ef 0120 70bd 6869  )h1`,`..(.. p.hi
+00005310: 0821 0843 6861 0020 70bd 0000 b40b 4000  .!.Cha. p.....@.
+00005320: f8b5 0500 0e00 1700 fff7 0eef 134a 1468  .............J.h
+00005330: 002c 17d0 d168 491c 00d1 0121 2368 1360  .,...hI....!#h.`
+00005340: 0023 2360 d160 e760 a660 6560 2361 6161  .##`.`.`.`e`#aaa
+00005350: 1189 491c 0904 090c 1181 5389 9942 08d9  ..I.......S..B..
+00005360: 5181 06e0 1169 1023 491c 1161 5169 1943  Q....i.#I..aQi.C
+00005370: 5161 fff7 f2ee 2000 f8bd 0000 b40b 4000  Qa.... .......@.
+00005380: 70b5 0500 084c 03d0 0120 2076 0a20 02e0  p....L...  v. ..
+00005390: 0020 2076 0720 00f0 85fb 226b 002a 02d0  .  v. ...."k.*..
+000053a0: 616b 2800 9047 70bd b40b 4000 70b5 0500  ak(..Gp...@.p...
+000053b0: 0329 01d9 0020 70bd c800 0949 4418 fff7  .)... p....ID...
+000053c0: c4ee a16f 7834 0029 02d1 6560 2560 02e0  ...ox4.)..e`%`..
+000053d0: 6168 0d60 6560 fff7 c0ee 0120 70bd 0000  ah.`e`..... p...
+000053e0: b40b 4000 10b5 1c00 fff7 9aff 0028 02d0  ..@..........(..
+000053f0: 2100 fff7 dbff 10bd f1b5 0025 2f00 82b0  !..........%/...
+00005400: 29e0 1748 e900 0e18 fff7 9eee b46f b767  )..H.........o.g
+00005410: fff7 a2ee 0194 11e0 6268 2668 e168 a068  ........bh&h.h.h
+00005420: 9047 fff7 92ee 0e49 0a68 2260 0c60 6761  .G.....I.h"`.`ga
+00005430: 0a89 521e 0a81 fff7 90ee 3400 002c ebd1  ..R.......4..,..
+00005440: 0198 0028 04d0 0298 0028 01d0 0025 02e0  ...(.....(...%..
+00005450: 6d1c 032d 03d8 0248 017e 0029 d1d0 febd  m..-...H.~.)....
+00005460: b40b 4000 0449 0222 0a76 1f23 ca6c 1b06  ..@..I.".v.#.l..
+00005470: 5a61 8863 7047 0000 b40b 4000 ca08 9200  Za.cpG....@.....
+00005480: 4907 8058 c90e c840 0007 000f 7047 0000  I..X...@....pG..
+00005490: 1c49 f8b5 4843 0721 030a 0320 4907 4860  .I..HC.!... I.H`
+000054a0: 0420 4860 184d 0022 6a60 184c 1000 4600  . H`.M."j`.L..F.
+000054b0: 8700 a65b 7f18 7e61 401c 0e28 f7d3 1448  ...[..~a@..(...H
+000054c0: c860 0b61 144b 1348 1860 0320 8004 8860  .`.a.K.H.`. ...`
+000054d0: 8a60 5802 8860 8860 1048 8860 0520 4004  .`X..`.`.H.`. @.
+000054e0: 8860 4a60 aa60 d803 6860 6424 03e0 0120  .`J`.`..h`d$... 
+000054f0: fff7 fcfd 641e 2868 4003 01d4 002c f6d1  ....d.(h@....,..
+00005500: 2000 f8bd cd07 0000 0003 00e0 2c58 0000   ...........,X..
+00005510: 1280 0100 e060 0000 0002 00e0 3300 0800  .....`......3...
+00005520: 0149 0820 c872 7047 207f 00e5 f3b5 81b0  .I. .rpG .......
+00005530: 0600 00d1 febd 1d48 4569 0720 fff7 18ee  .......HEi. ....
+00005540: 1a49 0023 2031 0c88 07e0 2701 ea5b a119  .I.# 1....'..[..
+00005550: 9142 09d9 2300 7919 4c88 002c f5d1 0721  .B..#.y.L..,...!
+00005560: fff7 18ee 2000 febd 9142 08d2 0e01 aa53  .... ....B.....S
+00005570: 2201 a952 7a19 5788 7619 7780 5180 002b  "..Rz.W.v.w.Q..+
+00005580: 06d0 2101 4919 1a01 4988 5219 5180 05e0  ..!.I...I.R.Q...
+00005590: 2101 064a 4919 4988 2032 1180 0299 0122  !..JI.I. 2....."
+000055a0: d203 1143 2201 5219 5180 d8e7 c07f 00e5  ...C".R.Q.......
+000055b0: f8b5 0026 0c48 4769 0b48 2030 0488 0620  ...&.HGi.H 0... 
+000055c0: fff7 d6ed 09e0 2101 7a5a 002a 03d0 151b  ......!.zZ.*....
+000055d0: b542 00d9 2e00 c919 4c88 002c f3d1 0621  .B......L..,...!
+000055e0: fff7 d8ed 3000 f8bd c07f 00e5 30b5 e124  ....0.......0..$
+000055f0: 0749 2406 e162 074b 0021 8a00 8558 9d50  .I$..b.K.!...X.P
+00005600: 491c 1029 f9d3 0248 c043 e062 30bd 0000  I..)...H.C.b0...
+00005610: 0000 ffff 0002 00e1 0148 406b 7047 0000  .........H@kpG..
+00005620: c07f 00e5 70b5 094e 7168 0402 0848 240a  ....p..Nqh...H$.
+00005630: 0d0e 4463 2d06 a009 00f0 b0fe a106 890e  ..Dc-...........
+00005640: 8001 0843 0543 7560 70bd 0000 8000 00e1  ...C.Cu`p.......
+00005650: c07f 00e5 f3b5 83b0 0700 2749 401e 8842  ..........'I@..B
+00005660: 47d2 2648 4569 0720 fff7 82ed 0190 2348  G.&HEi. ......#H
+00005670: 0499 2030 0488 3801 0026 0029 0290 0bd0  .. 0..8..&.)....
+00005680: 285a c11b 3800 00f0 71f8 05e0 a742 05d3  (Z..8...q....B..
+00005690: 2600 2001 4019 4488 002c f7d1 0298 3904  &. .@.D..,....9.
+000056a0: 4019 090c 002e 4480 03d0 3201 5219 5180  @.....D...2.R.Q.
+000056b0: 02e0 124a 2032 1180 002c 0ad0 0299 695a  ...J 2...,....iZ
+000056c0: a142 06d1 2101 6b5a 029a 4919 ab52 4988  .B..!.kZ..I..RI.
+000056d0: 4180 002e 09d0 3101 6a5a ba42 05d1 029a  A.....1.jZ.B....
+000056e0: aa5a 6a52 4088 4919 4880 0198 0721 fff7  .ZjR@.I.H....!..
+000056f0: 52ed 05b0 f0bd 0000 ff03 0000 c07f 00e5  R...............
+00005700: f3b5 81b0 0026 0700 0b48 4469 0120 c103  .....&...HDi. ..
+00005710: 0f43 0ae0 2919 4988 084a 1140 b942 03d1  .C..).I..J.@.B..
+00005720: 0299 fff7 97ff 761c 605b 0501 615b 0029  ......v.`[..a[.)
+00005730: f0d1 3000 febd 0000 c07f 00e5 ffe0 0000  ..0.............
+00005740: 10b5 0400 00f0 cef8 0020 00f0 3bf8 0548  ......... ..;..H
+00005750: fff7 4cff 0449 2002 0843 e121 0906 0860  ..L..I ..C.!...`
+00005760: 10bd 0000 4858 0000 0100 4000 f0b5 4518  ....HX....@...E.
+00005770: 0121 8902 8d42 01d9 0020 f0bd 0d49 0e4f  .!...B... ...I.O
+00005780: 4c69 0026 12e0 0d49 ff23 8200 1b06 5118  Li.&...I.#....Q.
+00005790: 0b60 0101 0919 4b60 094b d318 1e60 0023  .`....K`.K...`.#
+000057a0: db43 d219 ce60 1360 401c 8b60 8542 ead8  .C...`.`@..`.B..
+000057b0: 0120 f0bd c07f 00e5 0080 00e1 0040 00e1  . ...........@..
+000057c0: 00c0 00e1 10b5 0124 a402 211a fff7 ceff  .......$..!.....
+000057d0: 0848 084a 4069 0121 2032 1180 0021 0482  .H.J@i.! 2...!..
+000057e0: 2201 4182 8018 0180 4180 ff21 0906 4160  ".A.....A..!..A`
+000057f0: 10bd 0000 c07f 00e5 ffb5 0400 0e00 00d1  ................
+00005800: 6688 0120 8002 8642 09d8 1f06 0025 11e0  f.. ...B.....%..
+00005810: 2088 0299 4018 0121 8902 8842 02d3 0020   ...@..!...B... 
+00005820: 04b0 f0bd 6168 e268 cb19 a168 00f0 06f8  ....ah.h...h....
+00005830: 1034 6d1c b542 ebd3 0120 f1e7 ffb5 0600  .4m..B... ......
+00005840: 0120 0f00 8002 8642 02d3 0020 04b0 f0bd  . .....B... ....
+00005850: 1448 3101 4069 4418 180e 01d1 4020 007f  .H1.@iD.....@ ..
+00005860: 1d02 1149 2d0a 6560 0968 0902 0818 0121  ...I-.e`.h.....!
+00005870: c903 4018 6080 a809 00f0 90fd aa06 920e  ..@.`...........
+00005880: 8101 1143 094a b000 8218 1160 0849 094a  ...C.J.....`.I.J
+00005890: 4118 0f60 a760 0299 8018 0160 0120 e160  A..`.`.....`. .`
+000058a0: d4e7 0000 c07f 00e5 780b 4000 0040 00e1  ........x.@..@..
+000058b0: 0080 00e1 00c0 00e1 0122 c108 5203 9142  ........."..R..B
+000058c0: 01d3 0620 7047 4007 400f 4200 8018 044a  ... pG@.@.B....J
+000058d0: 8900 8918 0968 c140 4807 400f 7047 0000  .....h.@H.@.pG..
+000058e0: 0000 01e1 0649 074a 0020 0123 5b03 10b5  .....I.J. .#[...
+000058f0: 8400 a418 401c 9842 2160 f9d3 10bd 0000  ....@..B!`......
+00005900: b66d db00 0000 01e1 0123 c208 5b03 9a42  .m.......#..[..B
+00005910: 10b5 0dd2 4007 400f 4300 c018 9300 054a  ....@.@.C......J
+00005920: 0724 9a18 8440 1368 8140 a343 1943 1160  .$...@.h.@.C.C.`
+00005930: 10bd 0000 0000 01e1 4143 0448 0022 10b5  ........AC.H."..
+00005940: 8069 1300 00f0 8afb 10bd 0000 780b 4000  .i..........x.@.
+00005950: 0300 491e 02d0 8018 1860 f9e7 0021 1960  ..I......`...!.`
+00005960: 7047 1430 10b5 07c8 fff7 9cec 0020 10bd  pG.0......... ..
+00005970: 70b5 0300 8069 ff22 d969 0132 9042 01d8  p....i.".i.2.B..
+00005980: 0229 03d9 8420 1882 0020 70bd 5c69 1433  .)... ... p.\i.3
+00005990: 0029 06d1 02e0 625c 5a54 491c 8142 fad3  .)....b\ZTI..B..
+000059a0: 70bd 0129 09d1 0021 4508 03e0 4a00 a65a  p..)...!E...J..Z
+000059b0: 491c 9e52 8d42 f9d8 70bd 0021 8508 03e0  I..R.B..p..!....
+000059c0: 8a00 a658 491c 9e50 8d42 f9d8 70bd 0000  ...XI..P.B..p...
+000059d0: 10b5 0400 0d48 0088 0104 0d48 4268 0068  .....H.....HBh.h
+000059e0: 1202 8918 0818 6061 0a48 a061 0a48 0ba1  ......`a.H.a.H..
+000059f0: 0068 e061 2000 2030 fff7 14ec 2000 2f30  .h.a . 0.... ./0
+00005a00: 0aa1 fff7 10ec 2120 10bd 0000 007f 00e5  ......! ........
+00005a10: 780b 4000 0001 ffff 2058 0000 5341 524b  x.@..... X..SARK
+00005a20: 2f53 7069 4e4e 616b 6572 0000 332e 302e  /SpiNNaker..3.0.
+00005a30: 3100 0000 30b5 ff23 8269 c169 0133 9a42  1...0..#.i.i.3.B
+00005a40: 01d8 0229 02d9 8421 0182 1fe0 4369 2030  ...)...!....Ci 0
+00005a50: 0029 06d1 02e0 445c 5c54 491c 9142 fad3  .)....D\\TI..B..
+00005a60: 14e0 0129 09d1 0021 5408 03e0 4a00 855a  ...)...!T...J..Z
+00005a70: 491c 9d52 8c42 f9d8 08e0 0021 9408 03e0  I..R.B.....!....
+00005a80: 8a00 8558 491c 9d50 8c42 f9d8 0020 30bd  ...XI..P.B... 0.
+00005a90: 0021 02e0 491c 421e 1040 0028 fad1 0800  .!..I.B..@.(....
+00005aa0: 7047 0000 0249 c969 2031 8873 7047 0000  pG...I.i 1.spG..
+00005ab0: 780b 4000 0300 2de9 0202 a0e3 1400 90e5  x.@...-.........
+00005ac0: 1000 9fe5 3810 90e5 0110 81e2 3810 80e5  ....8.......8...
+00005ad0: 0300 bde8 04f0 5ee2 780b 4000 0200 1032  ......^.x.@....2
+00005ae0: 0839 8b1a 4260 083b 0161 c360 0260 0023  .9..B`.;.a.`.`.#
+00005af0: 8160 0b60 4361 4b60 7047 f8b5 0f00 0468  .`.`CaK`pG.....h
+00005b00: 0026 c907 0cd0 0620 fff7 32eb 08e0 2168  .&..... ..2...!h
+00005b10: 0029 04d0 0d1b 083d b542 00d9 2e00 6468  .).....=.B....dh
+00005b20: 002c f4d1 f907 02d0 0621 fff7 34eb 3000  .,.......!..4.0.
+00005b30: f8bd 0000 70b5 4025 2988 0400 8900 401a  ....p.@%).....@.
+00005b40: 6a88 d221 fff7 f4ea aa88 d121 fff7 f0ea  j..!.......!....
+00005b50: 0022 df21 fff7 ecea e888 8108 8900 611a  .".!..........a.
+00005b60: 344c 0020 2161 c06c 6061 fff7 b7ff a061  4L. !a.l`a.....a
+00005b70: 2806 4069 3049 000e 6060 4018 007d 2060  (.@i0I..``@..} `
+00005b80: 2d48 ff26 6038 8088 2086 2c48 2536 a060  -H.&`8.. .,H%6.`
+00005b90: 287e 3100 fff7 d0fe 2062 297e 3200 fff7  (~1..... b)~2...
+00005ba0: d7fe 7121 4906 6068 496b c906 c90e 8842  ..q!I.`hIk.....B
+00005bb0: 2dd0 2168 224a 204b c801 8018 403b e061  -.!h"J K....@;.a
+00005bc0: 9a69 4a43 9100 5a69 8918 6163 7022 0021  .iJC..Zi..acp".!
+00005bd0: fff7 68eb e069 0522 0100 2031 8a73 6268  ..h..i.".. 1.sbh
+00005be0: 4a73 2a7f ca73 1449 8039 c969 4164 1549  Js*..s.I.9.iAd.I
+00005bf0: c165 1549 4830 fff7 16eb 0f48 4030 c06b  .e.IH0.....H@0.k
+00005c00: 0002 000e 0328 02d0 1420 fbf7 90ea 00f0  .....(... ......
+00005c10: dbf9 687e 0d4b 0122 1221 00f0 f9f9 0c4b  ..h~.K.".!.....K
+00005c20: 0122 0621 1020 00f0 f3f9 a87e fff7 58fb  .".!. .....~..X.
+00005c30: 1f20 70bd 780b 4000 807f 00e5 adde adde  . p.x.@.........
+00005c40: 0070 00e5 0100 0300 2458 0000 e441 0000  .p......$X...A..
+00005c50: b44a 0000 f8b5 0121 524f 7a68 9140 524a  .J.....!ROzh.@RJ
+00005c60: 8918 7122 5206 d160 fb69 1c00 2034 217e  ..q"R..`.i.. 4!~
+00005c70: 0029 18d0 1a6b 0229 00d1 1863 0025 2576  .)...k.)...c.%%v
+00005c80: 1f26 3606 0329 20d1 d31e fff7 1eeb 0b11  .&6..) .........
+00005c90: 0c0c 0709 0d1c 1717 1717 0c00 0120 00e0  ............. ..
+00005ca0: 0020 fff7 6dfb f8bd ff20 fff7 dbfb f8bd  . ..m.... ......
+00005cb0: 4020 417f 4908 4900 4177 f8bd 3b48 c262  @ A.I.I.Aw..;H.b
+00005cc0: 0120 4007 67e0 1020 65e0 0129 f5d1 0092  . @.g.. e..)....
+00005cd0: 00f0 caf8 0400 60d0 0099 2000 fff7 b0ea  ......`... .....
+00005ce0: 0098 00f0 37f9 b86a 401c b862 a77a 3806  ....7..j@..b.z8.
+00005cf0: 400f 31d1 a088 1828 01d2 8120 1be0 208a  @.1....(... .. .
+00005d00: 8021 0028 2182 03d1 2000 fff7 61fe 14e0  .!.(!... ...a...
+00005d10: 0228 03d1 2000 fff7 2bfe 0ee0 0328 03d1  .(.. ...+....(..
+00005d20: 2000 fff7 87fe 08e0 0528 03d1 2000 fff7   ........(.. ...
+00005d30: 18fe 02e0 8320 2082 2800 0c30 a080 a07a  .....  .(..0...z
+00005d40: a189 e27a a272 e072 e089 a081 e181 0a21  ...z.r.r.......!
+00005d50: 2000 00f0 a3f8 13e0 4020 c07e 0028 13d0   .......@ .~.(..
+00005d60: 1348 8069 0028 0bd0 fff7 eee9 0500 7a09  .H.i.(........z.
+00005d70: 2100 0320 00f0 3cfa 2800 fff7 eee9 f8bd  !.. ..<.(.......
+00005d80: 2000 00f0 61f8 f8bd 3069 c000 f8d5 0748   ...a...0i.....H
+00005d90: 8462 0120 0007 b061 f8bd 0098 00f0 daf8  .b. ...a........
+00005da0: f8bd 0000 780b 4000 0000 c05e b40b 4000  ....x.@....^..@.
+00005db0: 380b 4000 f8b5 0021 0c48 fff7 5ffb 0600  8.@....!.H.._...
+00005dc0: 0024 0125 2f00 08e0 0848 2900 fff7 56fb  .$.%/....H)...V.
+00005dd0: 0100 3800 8840 0443 6d1c b542 f4d9 0448  ..8..@.Cm..B...H
+00005de0: 8460 4168 a143 4160 f8bd 0000 307f 00e5  .`Ah.CA`....0...
+00005df0: 4000 00e2 f8b5 0400 0021 1148 fff7 3efb  @........!.H..>.
+00005e00: 0700 104e 0125 18e0 0d48 2900 fff7 36fb  ...N.%...H)...6.
+00005e10: 0100 0120 8840 e107 2200 0223 c90f 1a40  ... .@.."..#...@
+00005e20: a408 002a 03d1 0029 06d0 3168 0140 0029  ...*...)..1h.@.)
+00005e30: 01d0 f060 00e0 b060 6d1c bd42 e4d9 f8bd  ...`...`m..B....
+00005e40: 307f 00e5 4000 00e2 70b5 0500 054c fff7  0...@...p....L..
+00005e50: 7ce9 216a 2960 2562 a18c 491e a184 fff7  |.!j)`%b..I.....
+00005e60: 7ce9 70bd 780b 4000 70b5 0b4c fff7 6ce9  |.p.x.@.p..L..l.
+00005e70: 256a 2034 002d 0ad0 2968 2160 a188 491c  %j 4.-..)h!`..I.
+00005e80: 0904 090c a180 e288 9142 00d9 e180 fff7  .........B......
+00005e90: 64e9 2800 70bd 0000 780b 4000 f8b5 0d00  d.(.p...x.@.....
+00005ea0: 0600 00f0 69f8 0400 01d1 0020 f8bd 3100  ....i...... ..1.
+00005eb0: 2000 fff7 c6e9 1c4e 0127 f069 4463 2030   ......N.'.iDc 0
+00005ec0: 4776 3800 fff7 54e9 3268 1849 3b00 9340  Gv8...T.2h.I;..@
+00005ed0: c96a 164a 0b43 0029 d362 08d1 1349 7122  .j.J.C.).b...Iq"
+00005ee0: 2039 097a 8f40 1249 7918 5206 9160 0121   9.z.@.Iy.R..`.!
+00005ef0: fff7 50e9 0d49 b039 0a68 f069 2030 03e0  ..P..I.9.h.i 0..
+00005f00: 0b68 9b1a ab42 02d8 437e 002b f8d1 407e  .h...B..C~.+..@~
+00005f10: 0028 03d0 2000 00f0 1df8 c6e7 f06a 401c  .(.. ........j@.
+00005f20: f062 0120 f8bd 0000 780b 4000 c07f 00e5  .b. ....x.@.....
+00005f30: 0000 c05e 0248 0b21 c069 2030 8173 7047  ...^.H.!.i 0.spG
+00005f40: 780b 4000 0248 0621 c069 2030 8173 7047  x.@..H.!.i 0.spG
+00005f50: 780b 4000 10b5 0400 0020 fff7 0ae9 0549  x.@...... .....I
+00005f60: 0a68 2260 0c60 8a88 521e 8a80 0021 fff7  .h"`.`..R....!..
+00005f70: 12e9 10bd 687f 00e5 0020 10b5 fff7 f8e8  ....h.... ......
+00005f80: 0949 0c68 002c 0ad0 2268 0a60 8a88 521c  .I.h.,.."h.`..R.
+00005f90: 1204 120c 8a80 cb88 9a42 00d9 ca80 0021  .........B.....!
+00005fa0: fff7 f8e8 2000 10bd 687f 00e5 0029 01d1  .... ...h....)..
+00005fb0: 4021 097f 034a 0902 d269 0818 8000 1058  @!...J...i.....X
+00005fc0: 7047 0000 c07f 00e5 0020 f0b5 c043 1f24  pG....... ...C.$
+00005fd0: 2406 6061 0022 e260 2263 074b 074d 084f  $.`a.".`"c.K.M.O
+00005fe0: 1000 8100 ce18 3260 c919 0d60 401c 1028  ......2`...`@..(
+00005ff0: f7d3 0448 6063 f0bd 0002 001f 0801 0000  ...H`c..........
+00006000: 0001 001f 1442 0000 01c0 8fe2 1cff 2fe1  .....B......../.
+00006010: 70b5 0124 8c40 1f25 2d06 1028 03d1 0020  p..$.@.%-..(... 
+00006020: c363 ec60 08e0 064e 8000 8619 3360 2023  .c.`...N....3` #
+00006030: 1943 044b c018 0160 002a 00d0 2c61 70bd  .C.K...`.*..,ap.
+00006040: 0001 001f 0002 001f 10b5 4024 01e0 fff7  ..........@$....
+00006050: f4e8 607f c007 fad1 10bd 0000 ffb5 81b0  ..`.............
+00006060: 0600 1d00 0029 32d0 0398 ff28 2fd8 280a  .....)2....(/.(.
+00006070: aa07 01d4 4020 007f 0202 0398 1018 0090  ....@ ..........
+00006080: 0398 0028 06d0 2848 009a c069 9200 8058  ...(..(H...i...X
+00006090: 0028 1cd1 c91c 8f08 bf00 0837 e807 03d0  .(.........7....
+000060a0: 0620 fff7 66e8 8446 3468 0022 07e0 2168  . ..f..F4h."..!h
+000060b0: e019 a042 05d9 8842 0cd9 2200 6468 002c  ...B...B..".dh.,
+000060c0: f5d1 e807 03d0 0621 6046 fff7 64e8 0020  .......!`F..d.. 
+000060d0: 05b0 f0bd 0300 0833 8b42 04d2 0160 2060  .......3.B...` `
+000060e0: 6168 4160 6060 6068 002a 01d0 5060 00e0  ahA````h.*..P`..
+000060f0: 3060 f068 c01b f060 e807 03d0 0621 6046  0`.h...`.....!`F
+00006100: fff7 48e8 0098 0121 0904 401a 6060 0398  ..H....!..@.``..
+00006110: 0028 06d0 0449 2000 ca69 0099 0830 8900  .(...I ..i...0..
+00006120: 5050 2000 0830 d3e7 c07f 00e5 f8b5 0500  PP ..0..........
+00006130: 0c00 1600 0029 02d1 1020 faf7 f8ef f007  .....)... ......
+00006140: 03d0 0620 fff7 14e8 0090 083c 6268 2868  ... .......<bh(h
+00006150: 1204 0021 120c 1306 04d0 184f 0023 ff69  ...!.......O.#.i
+00006160: 9200 bb50 2368 ea68 1b1b d218 ea60 03e0  ...P#h.h.....`..
+00006170: 8442 03d3 0100 4068 0028 f9d1 0029 6060  .B....@h.(...)``
+00006180: 01d0 4c60 00e0 2c60 0028 06d0 2268 8242  ..L`..,`.(.."h.B
+00006190: 03d1 0268 2260 4068 6060 0029 06d0 0868  ...h"`@h``.)...h
+000061a0: a042 03d1 2068 0860 6068 4860 f007 03d0  .B.. h.``hH`....
+000061b0: 0098 0621 fef7 eeef f8bd 0000 c07f 00e5  ...!............
+000061c0: f7b5 0700 0e00 4468 0025 0ce0 6068 0004  ......Dh.%..`h..
+000061d0: 000e 8642 06d1 2100 029a 0831 3800 fff7  ...B..!....18...
+000061e0: a5ff 6d1c 2468 2068 0028 efd1 2800 febd  ..m.$h h.(..(...
+000061f0: 7047 0000 01c0 8fe2 1cff 2fe1 10b5 0e4c  pG......../....L
+00006200: e369 1a64 d963 598f 0c4a 9142 01d0 491c  .i.d.cY..J.B..I.
+00006210: 5987 2168 0029 02d0 094a 1021 d172 0228  Y.!h.)...J.!.r.(
+00006220: 06d0 0028 07d1 0448 2030 807c 0028 02d0  ...(...H 0.|.(..
+00006230: 0d20 faf7 7cef 10bd 780b 4000 ffff 0000  . ..|...x.@.....
+00006240: 207f 00e5 2122 70b5 1206 d262 134d 0024   ...!"p....b.M.$
+00006250: 6868 2600 04e0 0168 6960 0460 0400 0800  hh&....hi`.`....
+00006260: 0028 14d0 0169 0029 f5d0 1162 0661 0ee0  .(...i.)...b.a..
+00006270: 6268 002a 02d0 e168 a068 9047 2068 2968  bh.*...h.h.G h)h
+00006280: 2160 2c60 6661 2989 491e 0400 2981 002c  !`,`fa).I...)..,
+00006290: eed1 1f20 0006 0063 70bd 0000 b40b 4000  ... ...cp.....@.
+000062a0: 0f50 2de9 e6ff fffa 0f50 bde8 04f0 5ee2  .P-......P....^.
+000062b0: 70b5 0400 0d00 0028 02d1 1020 faf7 36ef  p......(... ..6.
+000062c0: 6069 a842 23d1 fef7 40ef 114b 0025 5a68  `i.B#...@..K.%Zh
+000062d0: a242 01d1 6560 18e0 1168 14e0 a142 10d1  .B..e`...h...B..
+000062e0: 2168 1160 2168 0029 03d0 0a69 2669 9219  !h.`!h.)...i&i..
+000062f0: 0a61 1968 2160 1c60 6561 1989 491e 1981  .a.h!`.`ea..I...
+00006300: 03e0 0a00 0968 0029 e8d1 fef7 26ef 70bd  .....h.)....&.p.
+00006310: b40b 4000 f8b5 0400 1848 058e 4d43 fef7  ..@......H..MC..
+00006320: 14ef 1749 2122 4b68 1206 002b 04d1 4c60  ...I!"Kh...+..L`
+00006330: 1562 e321 9162 1ee0 576a bd42 05d2 1562  .b.!.b..Wj.B...b
+00006340: 7a1b 1a61 2360 4c60 15e0 0022 1600 1968  z..a#`L`..."...h
+00006350: ef1b 09e0 0d69 aa18 ba42 02d9 d21b 0a61  .....i...B.....a
+00006360: 04e0 0b00 0968 ae19 0029 f3d1 b91b 2161  .....h...)....!a
+00006370: 1968 2160 1c60 fef7 f0ee f8bd 780b 4000  .h!`.`......x.@.
+00006380: b40b 4000 10b5 1c00 fef7 caff 0028 03d0  ..@..........(..
+00006390: 2100 fff7 bfff 0120 10bd 0000 0200 70b5  !...... ......p.
+000063a0: 0020 084c 0100 0123 1d00 8d40 1542 04d0  . .L...#...@.B..
+000063b0: 0d19 2d7a 1e00 ae40 3043 491c 1229 f3d3  ..-z...@0CI..)..
+000063c0: 70bd 0000 a07f 00e5 ffff ffff ffff 0000  p...............
+000063d0: 0000 0000 0000 0000 ffff 0001 0100 0000  ................
+000063e0: 00ff ff00 0101 0000 0000 8200 0000 0000  ................
+000063f0: 0000 0000 0000 8200 0000 0000 0000 0000  ................
+00006400: 0000 0000 9630 0777 2c61 0eee ba51 0999  .....0.w,a...Q..
+00006410: 19c4 6d07 8ff4 6a70 35a5 63e9 a395 649e  ..m...jp5.c...d.
+00006420: 3288 db0e a4b8 dc79 1ee9 d5e0 88d9 d297  2......y........
+00006430: 2b4c b609 bd7c b17e 072d b8e7 911d bf90  +L...|.~.-......
+00006440: 6410 b71d f220 b06a 4871 b9f3 de41 be84  d.... .jHq...A..
+00006450: 7dd4 da1a ebe4 dd6d 51b5 d4f4 c785 d383  }......mQ.......
+00006460: 5698 6c13 c0a8 6b64 7af9 62fd ecc9 658a  V.l...kdz.b...e.
+00006470: 4f5c 0114 d96c 0663 633d 0ffa f50d 088d  O\...l.cc=......
+00006480: c820 6e3b 5e10 694c e441 60d5 7271 67a2  . n;^.iL.A`.rqg.
+00006490: d1e4 033c 47d4 044b fd85 0dd2 6bb5 0aa5  ...<G..K....k...
+000064a0: faa8 b535 6c98 b242 d6c9 bbdb 40f9 bcac  ...5l..B....@...
+000064b0: e36c d832 755c df45 cf0d d6dc 593d d1ab  .l.2u\.E....Y=..
+000064c0: ac30 d926 3a00 de51 8051 d7c8 1661 d0bf  .0.&:..Q.Q...a..
+000064d0: b5f4 b421 23c4 b356 9995 bacf 0fa5 bdb8  ...!#..V........
+000064e0: 9eb8 0228 0888 055f b2d9 0cc6 24e9 0bb1  ...(..._....$...
+000064f0: 877c 6f2f 114c 6858 ab1d 61c1 3d2d 66b6  .|o/.LhX..a.=-f.
+00006500: 9041 dc76 0671 db01 bc20 d298 2a10 d5ef  .A.v.q... ..*...
+00006510: 8985 b171 1fb5 b606 a5e4 bf9f 33d4 b8e8  ...q........3...
+00006520: a2c9 0778 34f9 000f 8ea8 0996 1898 0ee1  ...x4...........
+00006530: bb0d 6a7f 2d3d 6d08 976c 6491 015c 63e6  ..j.-=m..ld..\c.
+00006540: f451 6b6b 6261 6c1c d830 6585 4e00 62f2  .Qkkbal..0e.N.b.
+00006550: ed95 066c 7ba5 011b c1f4 0882 57c4 0ff5  ...l{.......W...
+00006560: c6d9 b065 50e9 b712 eab8 be8b 7c88 b9fc  ...eP.......|...
+00006570: df1d dd62 492d da15 f37c d38c 654c d4fb  ...bI-...|..eL..
+00006580: 5861 b24d ce51 b53a 7400 bca3 e230 bbd4  Xa.M.Q.:t....0..
+00006590: 41a5 df4a d795 d83d 6dc4 d1a4 fbf4 d6d3  A..J...=m.......
+000065a0: 6ae9 6943 fcd9 6e34 4688 67ad d0b8 60da  j.iC..n4F.g...`.
+000065b0: 732d 0444 e51d 0333 5f4c 0aaa c97c 0ddd  s-.D...3_L...|..
+000065c0: 3c71 0550 aa41 0227 1010 0bbe 8620 0cc9  <q.P.A.'..... ..
+000065d0: 25b5 6857 b385 6f20 09d4 66b9 9fe4 61ce  %.hW..o ..f...a.
+000065e0: 0ef9 de5e 98c9 d929 2298 d0b0 b4a8 d7c7  ...^...)".......
+000065f0: 173d b359 810d b42e 3b5c bdb7 ad6c bac0  .=.Y....;\...l..
+00006600: 2083 b8ed b6b3 bf9a 0ce2 b603 9ad2 b174   ..............t
+00006610: 3947 d5ea af77 d29d 1526 db04 8316 dc73  9G...w...&.....s
+00006620: 120b 63e3 843b 6494 3e6a 6d0d a85a 6a7a  ..c..;d.>jm..Zjz
+00006630: 0bcf 0ee4 9dff 0993 27ae 000a b19e 077d  ........'......}
+00006640: 4493 0ff0 d2a3 0887 68f2 011e fec2 0669  D.......h......i
+00006650: 5d57 62f7 cb67 6580 7136 6c19 e706 6b6e  ]Wb..ge.q6l...kn
+00006660: 761b d4fe e02b d389 5a7a da10 cc4a dd67  v....+..Zz...J.g
+00006670: 6fdf b9f9 f9ef be8e 43be b717 d58e b060  o.......C......`
+00006680: e8a3 d6d6 7e93 d1a1 c4c2 d838 52f2 df4f  ....~......8R..O
+00006690: f167 bbd1 6757 bca6 dd06 b53f 4b36 b248  .g..gW.....?K6.H
+000066a0: da2b 0dd8 4c1b 0aaf f64a 0336 607a 0441  .+..L....J.6`z.A
+000066b0: c3ef 60df 55df 67a8 ef8e 6e31 79be 6946  ..`.U.g...n1y.iF
+000066c0: 8cb3 61cb 1a83 66bc a0d2 6f25 36e2 6852  ..a...f...o%6.hR
+000066d0: 9577 0ccc 0347 0bbb b916 0222 2f26 0555  .w...G....."/&.U
+000066e0: be3b bac5 280b bdb2 925a b42b 046a b35c  .;..(....Z.+.j.\
+000066f0: a7ff d7c2 31cf d0b5 8b9e d92c 1dae de5b  ....1......,...[
+00006700: b0c2 649b 26f2 63ec 9ca3 6a75 0a93 6d02  ..d.&.c...ju..m.
+00006710: a906 099c 3f36 0eeb 8567 0772 1357 0005  ....?6...g.r.W..
+00006720: 824a bf95 147a b8e2 ae2b b17b 381b b60c  .J...z...+.{8...
+00006730: 9b8e d292 0dbe d5e5 b7ef dc7c 21df db0b  ...........|!...
+00006740: d4d2 d386 42e2 d4f1 f8b3 dd68 6e83 da1f  ....B......hn...
+00006750: cd16 be81 5b26 b9f6 e177 b06f 7747 b718  ....[&...w.owG..
+00006760: e65a 0888 706a 0fff ca3b 0666 5c0b 0111  .Z..pj...;.f\...
+00006770: ff9e 658f 69ae 62f8 d3ff 6b61 45cf 6c16  ..e.i.b...kaE.l.
+00006780: 78e2 0aa0 eed2 0dd7 5483 044e c2b3 0339  x.......T..N...9
+00006790: 6126 67a7 f716 60d0 4d47 6949 db77 6e3e  a&g...`.MGiI.wn>
+000067a0: 4a6a d1ae dc5a d6d9 660b df40 f03b d837  Jj...Z..f..@.;.7
+000067b0: 53ae bca9 c59e bbde 7fcf b247 e9ff b530  S..........G...0
+000067c0: 1cf2 bdbd 8ac2 baca 3093 b353 a6a3 b424  ........0..S...$
+000067d0: 0536 d0ba 9306 d7cd 2957 de54 bf67 d923  .6......)W.T.g.#
+000067e0: 2e7a 66b3 b84a 61c4 021b 685d 942b 6f2a  .zf..Ja...h].+o*
+000067f0: 37be 0bb4 a18e 0cc3 1bdf 055a 8def 022d  7..........Z...-
+00006800: 496e 2045 7665 7279 2044 7265 616d 2048  In Every Dream H
+00006810: 6f6d 6520 6120 4865 6172 7461 6368 6500  ome a Heartache.
+00006820: 4b3f 8f57 7363 616d 702d 3300 0600 0100  K?.Wscamp-3.....
+00006830: 0200 0700 0a00 0300 7502 0300 0200 0300  ........u.......
+00006840: 0100 0500 1700 1400 f17c fe01 f1bc fe01  .........|......
+00006850: f27c fe01 f2bc fe01 f47c fe01 f4bc fe01  .|.......|......
+00006860: f87c fe01 f8bc fe01 f1fc 0100 f2fc 0100  .|..............
+00006870: f4fc 0100 f8fc 0100 0000 0000 0000 0000  ................
+00006880: 0000 0000 0000 0000 adde adde 1000 0000  ................
+00006890: 0400 0000 0400 0000 0400 0000 fa00 0000  ................
+000068a0: b80b 0000 f401 0000 fa00 0000 0000 0000  ................
+000068b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000068c0: 0010 2030 4014 2434 4454 6474 0111 2131  .. 0@.$4DTdt..!1
+000068d0: 4151 2535 4555 6575 0212 2232 4252 6236  AQ%5EUeu.."2BRb6
+000068e0: 4656 6676 0313 2333 4353 6373 4757 6777  FVfv..#3CScsGWgw
+000068f0: 4014 2434 4454 6474 0010 2030 4151 2535  @.$4DTdt.. 0AQ%5
+00006900: 4555 6575 0111 2131 4252 6236 4656 6676  EUeu..!1BRb6FVfv
+00006910: 0212 2232 4353 6373 4757 6777 0313 2333  .."2CScsGWgw..#3
+00006920: 4454 6474 0010 2030 4014 2434 4555 6575  DTdt.. 0@.$4EUeu
+00006930: 0111 2131 4151 2535 4656 6676 0212 2232  ..!1AQ%5FVfv.."2
+00006940: 4252 6236 4757 6777 0313 2333 4353 6373  BRb6GWgw..#3CScs
+00006950: 0000 0000 0000 0000 0000 0000 0100 0000  ................
+00006960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006970: 3f00 0000 0900 0000 0000 0000 0000 0000  ?...............
+00006980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00006990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000069a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000069b0: 0000 0000 0000 0000 0000 0000            ............
```

## Comparing `SpiNNMan-2016.001/spinnman/messages/spinnaker_boot/_system_variables/_system_variable_boot_values.py` & `SpiNNMan-3.0.0/spinnman/messages/spinnaker_boot/_system_variables/_system_variable_boot_values.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from enum import Enum
 from collections import namedtuple
-from collections import OrderedDict
-from spinnman.model.machine_dimensions import MachineDimensions
 import struct
 
 _SYSTEM_VARIABLES_BOOT_SIZE = 128
 
 
 class _DataType(Enum):
     """ Enum for data types
     """
     BYTE = (1, "<B")
     SHORT = (2, "<H")
     INT = (4, "<I")
     LONG = (8, "<Q")
+    BYTE_ARRAY = (16, "s")
 
     def __new__(cls, value, struct_code, doc=""):
         obj = object.__new__(cls)
         obj._value_ = value
         obj._struct_code = struct_code
         return obj
 
@@ -64,29 +63,29 @@
         doc="The x-coordinate of the chip to send debug messages to")
     is_peer_to_peer_available = _Definition(
         _DataType.BYTE, offset=0x06,
         doc="Indicates if peer-to-peer is working on the chip")
     nearest_neighbour_last_id = _Definition(
         _DataType.BYTE, offset=0x07,
         doc="The last id used in nearest neighbour transaction")
-    nearest_ethernet_x = _Definition(
+    nearest_ethernet_y = _Definition(
         _DataType.BYTE, offset=0x08,
         doc="The x-coordinate of the nearest chip with Ethernet")
-    nearest_ethernet_y = _Definition(
+    nearest_ethernet_x = _Definition(
         _DataType.BYTE, offset=0x09,
         doc="The y-coordinate of the nearest chip with Ethernet")
     hardware_version = _Definition(
         _DataType.BYTE, offset=0x0a,
         doc="The version of the hardware in use")
     is_ethernet_available = _Definition(
         _DataType.BYTE, offset=0x0b,
         doc="Indicates if Ethernet is available on this chip")
-    links_available = _Definition(
+    p2p_b_repeats = _Definition(
         _DataType.BYTE, offset=0x0c,
-        doc="A bit-mask indicating which links are available")
+        doc="Number of times to send out P2PB packets")
     log_peer_to_peer_sequence_length = _Definition(
         _DataType.BYTE, offset=0x0d, default=4,
         doc="Log (base 2) of the peer-to-peer sequence length")
     clock_divisor = _Definition(
         _DataType.BYTE, offset=0x0e, default=0x33,
         doc="The clock divisors for system & router clocks")
     time_phase_scale = _Definition(
@@ -102,44 +101,54 @@
         _DataType.SHORT, offset=0x1a)
     unix_timestamp = _Definition(
         _DataType.INT, offset=0x1c,
         doc="The time in seconds since midnight, 1st January 1970")
     router_time_phase_timer = _Definition(
         _DataType.INT, offset=0x20,
         doc="The router time-phase timer")
-    cpu_clock_frequency_mhz = _Definition(
-        _DataType.SHORT, offset=0x24, default=150,
+    cpu_clock_mhz = _Definition(
+        _DataType.SHORT, offset=0x24, default=200,
         doc="The CPU clock frequency in MHz")
     sdram_clock_frequency_mhz = _Definition(
         _DataType.SHORT, offset=0x26, default=130,
         doc="The SDRAM clock frequency in MHz")
     nearest_neighbour_forward = _Definition(
         _DataType.BYTE, offset=0x28, default=0x3F,
         doc="Nearest-Neighbour forward parameter")
     nearest_neighbour_retry = _Definition(
         _DataType.BYTE, offset=0x29,
         doc="Nearest-Neighbour retry parameter")
     link_peek_timeout_microseconds = _Definition(
         _DataType.BYTE, offset=0x2a, default=100,
         doc="The link peek/poke timeout in microseconds")
     led_half_period_10_ms = _Definition(
-        _DataType.BYTE, offset=0x2b, default=50,
-        doc="The LED half-period in 10 ms units")
-    peer_to_peer_c_pkt_timer = _Definition(
-        _DataType.INT, offset=0x2c, default=0x010a6401,
-        doc="The peer-to-peer C packet timer")
+        _DataType.BYTE, offset=0x2b, default=1,
+        doc="The LED half-period in 10 ms units, or 1 to show load")
+    netinit_bc_wait_time = _Definition(
+        _DataType.BYTE, offset=0x2c, default=50,
+        doc="The time to wait after last BC during network initialisation"
+            " in 10 ms units")
+    netinit_phase = _Definition(
+        _DataType.BYTE, offset=0x2d, default=0,
+        doc="The phase of boot process (see enum netinit_phase_e)")
+    p2p_root_y = _Definition(
+        _DataType.BYTE, offset=0x2e, default=0,
+        doc="The y-coordinate of the chip from which the system was booted")
+    p2p_root_x = _Definition(
+        _DataType.BYTE, offset=0x2f, default=0,
+        doc="The x-coordinate of the chip from which the system was booted")
     led_0 = _Definition(
         _DataType.INT, offset=0x30, default=0x1,
         doc="The first part of the LED definitions")
     led_1 = _Definition(
-        _DataType.INT, offset=0x34,
+        _DataType.INT, offset=0x34, default=0,
         doc="The last part of the LED definitions")
-    peer_to_peer_b_pkt_timer = _Definition(
-        _DataType.INT, offset=0x38, default=0x01100a42,
-        doc="The peer-to-peer B packet timer")
+    padding_1 = _Definition(
+        _DataType.INT, offset=0x38, default=0,
+        doc="A word of padding")
     random_seed = _Definition(
         _DataType.INT, offset=0x3c,
         doc="The random seed")
     is_root_chip = _Definition(
         _DataType.BYTE, offset=0x40,
         doc="Indicates if this is the root chip")
     n_shared_message_buffers = _Definition(
@@ -147,114 +156,117 @@
         doc="The number of shared message buffers")
     nearest_neighbour_delay_us = _Definition(
         _DataType.BYTE, offset=0x42, default=10,
         doc="The delay between nearest-neighbour packets in microseconds")
     software_watchdog_count = _Definition(
         _DataType.BYTE, offset=0x43, default=3,
         doc="The number of watch dog timeouts before an error is raised")
-    probe_timer = _Definition(
-        _DataType.INT, offset=0x44, default=0x010a6401,
-        doc="The probe timer")
-    user_system_ram_size_words = _Definition(
+    padding_2 = _Definition(
+        _DataType.INT, offset=0x44, default=0,
+        doc="A word of padding")
+    system_ram_heap_address = _Definition(
         _DataType.INT, offset=0x48, default=1024,
-        doc="The size of the user system RAM heap in bytes")
-    user_sdram_size_words = _Definition(
+        doc="The base address of the system SDRAM heap")
+    sdram_heap_address = _Definition(
         _DataType.INT, offset=0x4c, default=0,
-        doc="The size of the user SDRAM heap in bytes")
-    iobuf_bytes = _Definition(
+        doc="The base address of the user SDRAM heap")
+    iobuf_size = _Definition(
         _DataType.INT, offset=0x50, default=16384,
         doc="The size of the iobuf buffer in bytes")
     system_sdram_bytes = _Definition(
         _DataType.INT, offset=0x54, default=8388608,
         doc="The size of the system SDRAM in bytes")
     system_buffer_words = _Definition(
         _DataType.INT, offset=0x58, default=32768,
         doc="The size of the system buffer in words")
     boot_signature = _Definition(
         _DataType.INT, offset=0x5c,
         doc="The boot signature")
     nearest_neighbour_memory_pointer = _Definition(
         _DataType.INT, offset=0x60,
         doc="The memory pointer for nearest neighbour global operations")
-    lock_0 = _Definition(
-        _DataType.BYTE, offset=0x64,
-        doc="The first lock")
-    lock_1 = _Definition(
-        _DataType.BYTE, offset=0x65,
-        doc="The second lock")
-    lock_2 = _Definition(
-        _DataType.BYTE, offset=0x66,
-        doc="The third lock")
+    lock = _Definition(
+        _DataType.BYTE, offset=0x64, default=0,
+        doc="The lock")
+    links_available = _Definition(
+        _DataType.BYTE, offset=0x65, default=0x3f,
+        doc="Bit mask (6 bits) of links enabled")
+    last_biff_id = _Definition(
+        _DataType.BYTE, offset=0x66, default=0,
+        doc="Last ID used in BIFF packet")
     board_test_flags = _Definition(
         _DataType.BYTE, offset=0x67,
         doc="Board testing flags")
     shared_message_first_free_address = _Definition(
         _DataType.INT, offset=0x68,
         doc="Pointer to the first free shared message buffer")
     shared_message_count_in_use = _Definition(
         _DataType.SHORT, offset=0x6c,
         doc="The number of shared message buffers in use")
     shared_message_maximum_used = _Definition(
         _DataType.SHORT, offset=0x6e,
         doc="The maximum number of shared message buffers used")
-    padding_1 = _Definition(
+    user_temp_0 = _Definition(
         _DataType.INT, offset=0x70,
-        doc="The first padding word")
-    padding_2 = _Definition(
+        doc="The first user variable")
+    user_temp_1 = _Definition(
         _DataType.INT, offset=0x74,
-        doc="The second padding word")
-    padding_3 = _Definition(
+        doc="The second user variable")
+    user_temp_2 = _Definition(
         _DataType.INT, offset=0x78,
-        doc="The third padding word")
-    padding_4 = _Definition(
+        doc="The third user variable")
+    user_temp_4 = _Definition(
         _DataType.INT, offset=0x7c,
-        doc="The fourth padding word")
+        doc="The fourth user variable")
     status_map = _Definition(
-        _DataType.BYTE, offset=0x80, array_size=20,
+        _DataType.BYTE_ARRAY, offset=0x80, array_size=20,
+        default=bytes(bytearray(20)),
         doc="The status map set during SCAMP boot")
     physical_to_virtual_core_map = _Definition(
-        _DataType.BYTE, offset=0x94, array_size=20,
+        _DataType.BYTE_ARRAY, offset=0x94, array_size=20,
+        default=bytes(bytearray(20)),
         doc="The physical core id to virtual core id map")
     virtual_to_physical_core_map = _Definition(
-        _DataType.BYTE, offset=0xa8, array_size=20,
+        _DataType.BYTE_ARRAY, offset=0xa8, array_size=20,
+        default=bytes(bytearray(20)),
         doc="The virtual core id to physical core id map")
     n_working_cores = _Definition(
         _DataType.BYTE, offset=0xbc,
         doc="The number of working cores")
     n_scamp_working_cores = _Definition(
         _DataType.BYTE, offset=0xbd,
         doc="The number of SCAMP working cores")
-    padding_5 = _Definition(
+    padding_3 = _Definition(
         _DataType.SHORT, offset=0xbe,
-        doc="The fifth padding short")
+        doc="A short of padding")
     sdram_base_address = _Definition(
         _DataType.INT, offset=0xc0,
         doc="The base address of SDRAM")
     system_ram_base_address = _Definition(
         _DataType.INT, offset=0xc4,
         doc="The base address of System RAM")
     system_sdram_base_address = _Definition(
         _DataType.INT, offset=0xc8,
         doc="The base address of System SDRAM")
     cpu_information_base_address = _Definition(
         _DataType.INT, offset=0xcc,
         doc="The base address of the cpu information blocks")
-    system_heap_sdram_base_address = _Definition(
+    system_sdram_heap_address = _Definition(
         _DataType.INT, offset=0xd0,
         doc="The base address of the system SDRAM heap")
-    routing_table_copy_address = _Definition(
+    router_table_copy_address = _Definition(
         _DataType.INT, offset=0xd4,
         doc="The address of the copy of the routing tables")
     peer_to_peer_hop_table_address = _Definition(
         _DataType.INT, offset=0xd8,
         doc="The address of the peer-to-peer hop tables")
     allocated_tag_table_address = _Definition(
         _DataType.INT, offset=0xdc,
         doc="The address of the allocated tag table")
-    router_first_free_entry = _Definition(
+    first_free_router_entry = _Definition(
         _DataType.SHORT, offset=0xe0,
         doc="The id of the first free router entry")
     n_active_peer_to_peer_addresses = _Definition(
         _DataType.SHORT, offset=0xe2,
         doc="The number of active peer-to-peer addresses")
     app_data_table_address = _Definition(
         _DataType.INT, offset=0xe4,
@@ -262,25 +274,26 @@
     shared_message_buffer_address = _Definition(
         _DataType.INT, offset=0xe8,
         doc="The address of the shared message buffers")
     monitor_mailbox_flags = _Definition(
         _DataType.INT, offset=0xec,
         doc="The monitor incoming mailbox flags")
     ethernet_ip_address = _Definition(
-        _DataType.BYTE, offset=0xf0, array_size=4,
+        _DataType.BYTE_ARRAY, offset=0xf0, array_size=4,
+        default=bytes(bytearray(4)),
         doc="The ip address of the chip")
-    user_temp_1 = _Definition(
+    fixed_route_copy = _Definition(
         _DataType.INT, offset=0xf4,
-        doc="The first user variable")
-    user_temp_2 = _Definition(
+        doc="A (virtual) copy of the router FR register")
+    board_info = _Definition(
         _DataType.INT, offset=0xf8,
-        doc="The second user variable")
-    user_temp_3 = _Definition(
+        doc="A pointer to the board information structure")
+    padding_4 = _Definition(
         _DataType.INT, offset=0xfc,
-        doc="The third user variable")
+        doc="A word of padding")
 
     def __init__(self, offset, data_type, default, array_size, doc):
         """
 
         :param data_type: The data type of the variable
         :type data_type: :py:class:`_DataType`
         :param offset: The offset from the start of the system variable\
@@ -299,66 +312,59 @@
         self.__doc__ = doc
 
     @property
     def data_type(self):
         return self._data_type
 
     @property
+    def array_size(self):
+        return self._array_size
+
+    @property
     def offset(self):
         return self._offset
 
     @property
     def default(self):
         return self._default
 
 
 class SystemVariableBootValues(object):
     """ Default values of the system variables that get passed to SpiNNaker\
         during boot
     """
 
-    def __init__(self, hardware_version, cpu_clock_frequency_mhz, led_0):
+    def __init__(self, hardware_version=None, led_0=None):
 
         # Create a dict of variable values
         self._values = dict()
         for variable in SystemVariableDefinition:
             self._values[variable] = variable.default
 
-        self._values[SystemVariableDefinition.hardware_version] =\
-            hardware_version
-        self._values[SystemVariableDefinition.cpu_clock_frequency_mhz] =\
-            cpu_clock_frequency_mhz
-        self._values[SystemVariableDefinition.led_0] = led_0
+        if hardware_version is not None:
+            self._values[SystemVariableDefinition.hardware_version] =\
+                hardware_version
+        if led_0 is not None:
+            self._values[SystemVariableDefinition.led_0] = led_0
 
     def set_value(self, system_variable_definition, value):
         self._values[system_variable_definition] = value
 
     @property
     def bytestring(self):
         data = b""
         for sys_var in SystemVariableDefinition:
             data += struct.pack(sys_var.data_type.struct_code,
                                 self._values[sys_var])
         return data
 
 spinnaker_boot_values = {
     1: SystemVariableBootValues(
-        hardware_version=1, cpu_clock_frequency_mhz=200, led_0=0x00076104),
+        hardware_version=1, led_0=0x00076104),
     2: SystemVariableBootValues(
-        hardware_version=2, cpu_clock_frequency_mhz=200, led_0=0x00006103),
+        hardware_version=2, led_0=0x00006103),
     3: SystemVariableBootValues(
-        hardware_version=3, cpu_clock_frequency_mhz=200, led_0=0x00000502),
+        hardware_version=3, led_0=0x00000502),
     4: SystemVariableBootValues(
-        hardware_version=4, cpu_clock_frequency_mhz=200, led_0=0x00000001),
+        hardware_version=4, led_0=0x00000001),
     5: SystemVariableBootValues(
-        hardware_version=5, cpu_clock_frequency_mhz=200, led_0=0x00000001)}
-
-spinnaker_standard_board_to_machine_sizes = {
-    1: MachineDimensions(2, 2),
-    2: MachineDimensions(2, 2),
-    3: MachineDimensions(2, 2),
-    4: MachineDimensions(8, 8),
-    5: MachineDimensions(8, 8)}
-
-# Can be used to enable extra things on larger machines
-# (but not currently used)
-spinnaker_multi_board_extra_configs = OrderedDict()
+        hardware_version=5, led_0=0x00000001)}
```

## Comparing `SpiNNMan-2016.001/spinnman/model/adc_info.py` & `SpiNNMan-3.0.0/spinnman/model/adc_info.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/model/bmp_connection_data.py` & `SpiNNMan-3.0.0/spinnman/model/bmp_connection_data.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/model/cpu_info.py` & `SpiNNMan-3.0.0/spinnman/model/cpu_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,29 +27,28 @@
         self._x = x
         self._y = y
         self._p = p
 
         (registers,                                                  # 32s 0
          self._processor_state_register, self._stack_pointer,
          self._link_register,                                        # 3I  32
-         run_time_error,                                             # B   44
-         # skipped                                                   # x   45
+         run_time_error, self._physical_cpu_id,                      # 2B  44
          state, self._application_id,                                # 2B  46
          self._application_mailbox_data_address,
          self._monitor_mailbox_data_address,                         # 2I  48
          application_mailbox_command, monitor_mailbox_command,       # 2B  56
          self._software_error_count,                                 # H   58
          self._software_source_filename_address,
          self._software_source_line_number, self._time,              # 3I  60
          self._application_name,                                     # 16s 72
-         self._iobuf_address,                                        # I   88
-         # skipped                                                   # 20x 92
+         self._iobuf_address, self._software_version,                # 2I  88
+         # skipped                                                   # 16x 96
          user0, user1, user2, user3                                  # 4I  112
-         ) = struct.unpack_from("< 32s 3I B x 2B 2I 2B H 3I 16s I 20x 4I",
-                                cpu_data, offset)
+         ) = struct.unpack_from(
+             "< 32s 3I 2B 2B 2I 2B H 3I 16s 2I 16x 4I", cpu_data, offset)
 
         index = self._application_name.find('\0')
         if index != -1:
             self._application_name = self._application_name[0:index]
 
         self._registers = [struct.unpack_from("<I", registers, i)
                            for i in range(0, 32, 4)]
@@ -95,14 +94,23 @@
 
         :return: The state of the core
         :rtype: :py:class:`spinnman.model.cpu_state.CPUState`
         """
         return self._state
 
     @property
+    def physical_cpu_id(self):
+        """ The physical id of this processor
+
+        :return: The physical id of the processor
+        :rtype: int
+        """
+        return self._physical_cpu_id
+
+    @property
     def application_name(self):
         """ The name of the application running on the core
 
         :return: The name of the application
         :rtype: str
         """
         return self._application_name
@@ -197,35 +205,35 @@
         :return: The line number
         :rtype: int
         """
         return self._software_source_line_number
 
     @property
     def processor_state_register(self):
-        """ The value in the processor state register (psr)
+        """ The value in the processor state register (PSR)
 
-        :return: The psr value
+        :return: The PSR value
         :rtype: int
         """
         return self._processor_state_register
 
     @property
     def stack_pointer(self):
-        """ The current stack pointer value (sp)
+        """ The current stack pointer value (SP)
 
-        :return: The sp value
+        :return: The SP value
         :rtype: int
         """
         return self._stack_pointer
 
     @property
     def link_register(self):
-        """ The current link register value (lr)
+        """ The current link register value (LR)
 
-        :return: The lr value
+        :return: The LR value
         :rtype: int
         """
         return self._link_register
 
     @property
     def registers(self):
         """ The current register values (r0 - r7)
@@ -249,11 +257,20 @@
         """ The address of the IOBUF buffer in SDRAM
 
         :return: The address
         :rtype: int
         """
         return self._iobuf_address
 
+    @property
+    def software_version(self):
+        """ The software version
+
+        :return: The software version
+        :rtype: int
+        """
+        return self._software_version
+
     def __str__(self):
         return "{}:{}:{:02n} {:18} {:16s} {:3n}".format(
             self.x, self.y, self.p, self._state.name, self._application_name,
             self._application_id)
```

## Comparing `SpiNNMan-2016.001/spinnman/model/cpu_state.py` & `SpiNNMan-3.0.0/spinnman/model/cpu_state.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/model/diagnostic_filter.py` & `SpiNNMan-3.0.0/spinnman/model/diagnostic_filter.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/model/diagnostic_filter_default_routing_status.py` & `SpiNNMan-3.0.0/spinnman/model/diagnostic_filter_default_routing_status.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/model/diagnostic_filter_destination.py` & `SpiNNMan-3.0.0/spinnman/model/diagnostic_filter_destination.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/model/diagnostic_filter_emergency_routing_status.py` & `SpiNNMan-3.0.0/spinnman/model/diagnostic_filter_emergency_routing_status.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/model/diagnostic_filter_packet_type.py` & `SpiNNMan-3.0.0/spinnman/model/diagnostic_filter_packet_type.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/model/diagnostic_filter_payload_status.py` & `SpiNNMan-3.0.0/spinnman/model/diagnostic_filter_payload_status.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/model/dpri_status.py` & `SpiNNMan-3.0.0/spinnman/model/dpri_status.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/model/io_buffer.py` & `SpiNNMan-3.0.0/spinnman/model/io_buffer.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/model/machine_dimensions.py` & `SpiNNMan-3.0.0/spinnman/model/machine_dimensions.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/model/mailbox_command.py` & `SpiNNMan-3.0.0/spinnman/model/mailbox_command.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/model/router_diagnostics.py` & `SpiNNMan-3.0.0/spinnman/model/router_diagnostics.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/model/version_info.py` & `SpiNNMan-3.0.0/spinnman/model/version_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from spinnman.exceptions import SpinnmanInvalidParameterException
 from time import localtime
 from time import asctime
 import struct
+import re
+from spinnman import exceptions
 
 
 class VersionInfo(object):
     """ Decodes SC&MP/SARK version information as returned by the SVER command
     """
 
     def __init__(self, version_data, offset=0):
@@ -14,24 +16,38 @@
                     information
         :param offset: the offset in the bytes from an SCP packet containing
                        version information
         :type version_data: bytearray
         :raise spinnman.exceptions.SpinnmanInvalidParameterException: If the\
                     message does not contain valid version information
         """
-        (self._p, self._y, self._x, version_no, self._build_date) = \
-            struct.unpack_from("<BxBB2xHI", version_data, offset)
-        self._version_number = version_no / 100.0
-        self._version_string = version_data[offset + 12:-1].decode("ascii")
-        try:
-            self._name, self._hardware = self._version_string.split("/")
-        except ValueError as exception:
-            raise SpinnmanInvalidParameterException(
-                "version_string", self._version_string,
-                "Incorrect format: {}".format(exception))
+        (self._p, self._physical_cpu_id, self._y, self._x, _,
+            version_no, self._build_date) = struct.unpack_from(
+                "<BBBBHHI", version_data, offset)
+
+        version_data = version_data[offset + 12:-1].decode("utf-8")
+
+        if version_no < 0xFFFF:
+            try:
+                self._version_number = (version_no // 100, version_no % 100, 0)
+                self._name, self._hardware = version_data.split("/")
+                self._version_string = version_data
+            except ValueError as exception:
+                raise SpinnmanInvalidParameterException(
+                    "version_data", self._version_string,
+                    "Incorrect format: {}".format(exception))
+        else:
+            name_hardware, _, version = version_data.partition("\0")
+            self._version_string = version
+            matches = re.match("(\d+)\.(\d+)\.(\d+)", version)
+            if matches is None:
+                raise exceptions.SpinnmanInvalidParameterException(
+                    "version", version, "Cannot be parsed")
+            self._version_number = tuple(map(int, matches.group(1, 2, 3)))
+            self._name, self._hardware = name_hardware.rstrip("\0").split("/")
 
     @property
     def name(self):
         """ The name of the software
 
         :return: The name
         :rtype: str
@@ -100,9 +116,9 @@
         :return: The version information
         :rtype: str
         """
         return self._version_string
 
     def __str__(self):
         return "[Version: {} {} at {}:{}:{}:{} (built {})]".format(
-            self._name, self._version_number, self._hardware, self._x, self._y,
+            self._name, self._version_string, self._hardware, self._x, self._y,
             self._p, asctime(localtime(self._build_date)))
```

## Comparing `SpiNNMan-2016.001/spinnman/processes/abstract_multi_connection_process.py` & `SpiNNMan-3.0.0/spinnman/processes/abstract_multi_connection_process.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/abstract_multi_connection_process_connection_selector.py` & `SpiNNMan-3.0.0/spinnman/processes/abstract_multi_connection_process_connection_selector.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/abstract_process.py` & `SpiNNMan-3.0.0/spinnman/processes/abstract_process.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/abstract_single_connection_process.py` & `SpiNNMan-3.0.0/spinnman/processes/abstract_single_connection_process.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/application_run_process.py` & `SpiNNMan-3.0.0/spinnman/processes/application_run_process.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/de_alloc_sdram_process.py` & `SpiNNMan-3.0.0/spinnman/processes/de_alloc_sdram_process.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/exit_dpri_process.py` & `SpiNNMan-3.0.0/spinnman/processes/exit_dpri_process.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/get_routes_process.py` & `SpiNNMan-3.0.0/spinnman/processes/get_routes_process.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/get_tags_process.py` & `SpiNNMan-3.0.0/spinnman/processes/get_tags_process.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/get_version_process.py` & `SpiNNMan-3.0.0/spinnman/processes/get_version_process.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/load_routes_process.py` & `SpiNNMan-3.0.0/spinnman/processes/load_routes_process.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/malloc_sdram_process.py` & `SpiNNMan-3.0.0/spinnman/processes/malloc_sdram_process.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/multi_connection_process_most_direct_connection_selector.py` & `SpiNNMan-3.0.0/spinnman/processes/multi_connection_process_most_direct_connection_selector.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/multi_connection_process_round_robin_connection_selector.py` & `SpiNNMan-3.0.0/spinnman/processes/multi_connection_process_round_robin_connection_selector.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/read_dpri_status_process.py` & `SpiNNMan-3.0.0/spinnman/processes/read_dpri_status_process.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/read_iobuf_process.py` & `SpiNNMan-3.0.0/spinnman/processes/read_iobuf_process.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,54 @@
 import functools
 import struct
 from collections import defaultdict
 from collections import OrderedDict
 
-from spinnman.processes.get_cpu_info_process import GetCPUInfoProcess
 from spinnman.model.io_buffer import IOBuffer
+from spinnman.utilities import utility_functions
 from spinnman.messages.scp.impl.scp_read_memory_request \
     import SCPReadMemoryRequest
 from spinnman.processes.abstract_multi_connection_process \
     import AbstractMultiConnectionProcess
 from spinnman import constants
 
 
 class ReadIOBufProcess(AbstractMultiConnectionProcess):
     """ A process for reading memory
     """
 
     def __init__(self, connection_selector):
         AbstractMultiConnectionProcess.__init__(self, connection_selector)
 
+        # A dictionary of (x, y, p) -> iobuf address
+        self._iobuf_address = dict()
+
         # A dictionary of (x, y, p) -> OrderedDict(n) -> bytearray
         self._iobuf = defaultdict(OrderedDict)
 
         # A dictionary of (x, y, p) -> OrderedDict(n) -> memoryview
         self._iobuf_view = defaultdict(OrderedDict)
 
         # A list of extra reads that need to be done as a result of the first
         # read = list of (x, y, p, n, base_address, size, offset)
         self._extra_reads = list()
 
         # A list of next reads that need to be done as a result of the first
         # read = list of (x, y, p, n, next_address, first_read_size)
         self._next_reads = list()
 
+    def handle_iobuf_address_response(self, iobuf_size, x, y, p, response):
+        iobuf_address = struct.unpack_from(
+            "<I", response.data, response.offset)[0]
+        if iobuf_address != 0:
+            first_read_size = min(
+                (iobuf_size + 16, constants.UDP_MESSAGE_MAX_SIZE))
+            self._next_reads.append((
+                x, y, p, 0, iobuf_address, first_read_size))
+
     def handle_first_iobuf_response(self, x, y, p, n, base_address,
                                     first_read_size, response):
 
         # Unpack the iobuf header
         (next_address, bytes_to_read) = struct.unpack_from(
             "<I8xI", response.data, response.offset)
 
@@ -77,30 +89,31 @@
                                      first_read_size))
 
     def handle_extra_iobuf_response(self, x, y, p, n, offset, response):
         view = self._iobuf_view[(x, y, p)][n]
         view[offset:offset + response.length] = response.data[
             response.offset:response.offset + response.length]
 
-    def read_iobuf(self, chip_info, core_subsets):
-        cpu_info_process = GetCPUInfoProcess(self._next_connection_selector)
-        cpu_information = cpu_info_process.get_cpu_info(chip_info,
-                                                        core_subsets)
-
-        # Kick-start the reading of the IOBufs
-        for cpu_info in cpu_information:
-            this_chip_info = chip_info[(cpu_info.x, cpu_info.y)]
-            if cpu_info.iobuf_address != 0:
-                iobuf_size = this_chip_info.iobuf_size + 16
-                first_read_size = min(
-                    (iobuf_size, constants.UDP_MESSAGE_MAX_SIZE))
-
-                self._next_reads.append((
-                    cpu_info.x, cpu_info.y, cpu_info.p, 0,
-                    cpu_info.iobuf_address, first_read_size))
+    def read_iobuf(self, iobuf_size, core_subsets):
+
+        # Get the iobuf address for each core
+        for core_subset in core_subsets:
+            x = core_subset.x
+            y = core_subset.y
+            for p in core_subset.processor_ids:
+                base_address = (
+                    utility_functions.get_vcpu_address(p) +
+                    constants.CPU_IOBUF_ADDRESS_OFFSET)
+                self._send_request(
+                    SCPReadMemoryRequest(x, y, base_address, 4),
+                    functools.partial(
+                        self.handle_iobuf_address_response,
+                        iobuf_size, x, y, p))
+        self._finish()
+        self.check_for_error()
 
         # Run rounds of the process until reading is complete
         while len(self._extra_reads) > 0 or len(self._next_reads) > 0:
 
             # Process the extra iobuf reads needed
             while len(self._extra_reads) > 0:
                 (x, y, p, n, base_address, size, offset) = \
```

## Comparing `SpiNNMan-2016.001/spinnman/processes/read_memory_process.py` & `SpiNNMan-3.0.0/spinnman/processes/read_memory_process.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/read_router_diagnostics_process.py` & `SpiNNMan-3.0.0/spinnman/processes/read_router_diagnostics_process.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/reset_dpri_counters_process.py` & `SpiNNMan-3.0.0/spinnman/processes/reset_dpri_counters_process.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/send_single_command_process.py` & `SpiNNMan-3.0.0/spinnman/processes/send_single_command_process.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/set_dpri_packet_types_process.py` & `SpiNNMan-3.0.0/spinnman/processes/set_dpri_packet_types_process.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/set_dpri_router_emergency_timeout_process.py` & `SpiNNMan-3.0.0/spinnman/processes/set_dpri_router_emergency_timeout_process.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/set_dpri_router_timeout_process.py` & `SpiNNMan-3.0.0/spinnman/processes/set_dpri_router_timeout_process.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/write_memory_flood_process.py` & `SpiNNMan-3.0.0/spinnman/processes/write_memory_flood_process.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/processes/write_memory_process.py` & `SpiNNMan-3.0.0/spinnman/processes/write_memory_process.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/utilities/locate_connected_machine_ip_address.py` & `SpiNNMan-3.0.0/spinnman/utilities/locate_connected_machine_ip_address.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/spinnman/utilities/reports.py` & `SpiNNMan-3.0.0/spinnman/utilities/reports.py`

 * *Files identical despite different names*

## Comparing `SpiNNMan-2016.001/SpiNNMan.egg-info/SOURCES.txt` & `SpiNNMan-3.0.0/SpiNNMan.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,16 @@
 spinnman/messages/scp/abstract_messages/abstract_scp_response.py
 spinnman/messages/scp/impl/__init__.py
 spinnman/messages/scp/impl/scp_app_stop_request.py
 spinnman/messages/scp/impl/scp_application_run_request.py
 spinnman/messages/scp/impl/scp_bmp_set_led_request.py
 spinnman/messages/scp/impl/scp_bmp_version_request.py
 spinnman/messages/scp/impl/scp_check_ok_response.py
+spinnman/messages/scp/impl/scp_chip_info_request.py
+spinnman/messages/scp/impl/scp_chip_info_response.py
 spinnman/messages/scp/impl/scp_count_state_request.py
 spinnman/messages/scp/impl/scp_count_state_response.py
 spinnman/messages/scp/impl/scp_dpri_exit_request.py
 spinnman/messages/scp/impl/scp_dpri_get_status_request.py
 spinnman/messages/scp/impl/scp_dpri_get_status_response.py
 spinnman/messages/scp/impl/scp_dpri_reset_counters_request.py
 spinnman/messages/scp/impl/scp_dpri_set_reinjection_packet_types.py
@@ -179,46 +181,46 @@
 spinnman/messages/sdp/sdp_message.py
 spinnman/messages/spinnaker_boot/__init__.py
 spinnman/messages/spinnaker_boot/spinnaker_boot_message.py
 spinnman/messages/spinnaker_boot/spinnaker_boot_messages.py
 spinnman/messages/spinnaker_boot/spinnaker_boot_op_code.py
 spinnman/messages/spinnaker_boot/_system_variables/__init__.py
 spinnman/messages/spinnaker_boot/_system_variables/_system_variable_boot_values.py
-spinnman/messages/spinnaker_boot/boot_data/scamp-133.boot
+spinnman/messages/spinnaker_boot/boot_data/scamp-3.boot
 spinnman/model/__init__.py
 spinnman/model/adc_info.py
 spinnman/model/bmp_connection_data.py
 spinnman/model/chip_info.py
-spinnman/model/core_subset.py
-spinnman/model/core_subsets.py
+spinnman/model/chip_summary_info.py
 spinnman/model/cpu_info.py
 spinnman/model/cpu_state.py
 spinnman/model/diagnostic_filter.py
 spinnman/model/diagnostic_filter_default_routing_status.py
 spinnman/model/diagnostic_filter_destination.py
 spinnman/model/diagnostic_filter_emergency_routing_status.py
 spinnman/model/diagnostic_filter_packet_type.py
 spinnman/model/diagnostic_filter_payload_status.py
 spinnman/model/diagnostic_filter_source.py
 spinnman/model/dpri_status.py
 spinnman/model/io_buffer.py
 spinnman/model/machine_dimensions.py
 spinnman/model/mailbox_command.py
+spinnman/model/p2p_table.py
+spinnman/model/p2p_table_route.py
 spinnman/model/router_diagnostics.py
 spinnman/model/run_time_error.py
 spinnman/model/version_info.py
 spinnman/model_binaries/__init__.py
 spinnman/model_binaries/reinjector.aplx
 spinnman/processes/__init__.py
 spinnman/processes/abstract_multi_connection_process.py
 spinnman/processes/abstract_multi_connection_process_connection_selector.py
 spinnman/processes/abstract_process.py
 spinnman/processes/abstract_single_connection_process.py
 spinnman/processes/application_run_process.py
-spinnman/processes/check_machine_booted_process.py
 spinnman/processes/de_alloc_sdram_process.py
 spinnman/processes/exit_dpri_process.py
 spinnman/processes/get_cpu_info_process.py
 spinnman/processes/get_machine_process.py
 spinnman/processes/get_routes_process.py
 spinnman/processes/get_tags_process.py
 spinnman/processes/get_version_process.py
```

