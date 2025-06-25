# Changelog

This document provides a high-level view of the changes to the macOS Security Compliance Project.

## [Ventura, Revision 5.2] - 2025-06-XX

* Rules
  * Modified Rules
    * audit_auditd_enabled
    * auth_ssh_password_authentication_disable
    * os_anti_virus_installed
    * os_authenticated_root_enable
    * os_hibernate_mode_intel_enable
    * os_parental_controls_enable
    * os_policy_banner_ssh_enforce
    * os_separate_functionality
    * os_ssh_server_alive_count_max_configure
    * os_ssh_server_alive_interval_configure
    * os_sshd_client_alive_count_max_configure
    * os_sshd_client_alive_interval_configure
    * os_sshd_fips_compliant
    * os_sshd_login_grace_time_configure
    * os_sshd_permit_root_login_configure
    * os_time_server_enabled
    * os_world_writable_system_folder_configure
    * pwpolicy_account_inactivity_enforce
    * pwpolicy_temporary_or_emergency_accounts_disable
    * system_settings_location_services_disable
    * system_settings_location_services_enable
    * system_settings_media_sharing_disabled
    * system_settings_software_update_enforce
    * system_settings_time_server_configure
    * system_settings_time_server_enforce
* Scripts
  * generate_guidance
    * bug fixes
  * generate_scap
    * bug fixes

## [Ventura, Revision 5.1] - 2024-12-16

* Rules
  * Modified Rules
    * os_world_writable_library_folder_configure
    * pwpolicy_special_character_enforce
    * pwpolicy_history_enforce
    * pwpolicy_account_lockout_timeout_enforce
    * pwpolicy_account_lockout_enforce

## [Ventura, Revision 5.0] - 2024-09-12

* Rules
  * Modified Rules
    * os_application_sandboxing (https://github.com/usnistgov/macos_security/pull/409[#409])
    * os_camera_disable (https://github.com/usnistgov/macos_security/issues/388[#388])
    * os_mobile_file_integrity_enable (https://github.com/usnistgov/macos_security/pull/409[#409])
    * system_settings_rae_disable (https://github.com/usnistgov/macos_security/pull/408[#408])
    * system_settings_siri_listen_disable (https://github.com/usnistgov/macos_security/issues/411[#411])
    * system_settings_ssh_disable (https://github.com/usnistgov/macos_security/pull/408[#408])
    * system_settings_system_wide_preferences_configure (https://github.com/usnistgov/macos_security/issues/418[#418])
  * Removed Rules
    * os_safari_popups_disabled
* Baselines
  * Modified existing baselines

* Scripts
  * generate_guidance
    * Updated date format for compliance script (https://github.com/usnistgov/macos_security/issues/405[#405])
    * Spelling fixes (https://github.com/usnistgov/macos_security/pull/409[#409])
    * Support `.yaml` & .`yml` (https://github.com/usnistgov/macos_security/issues/412[#412])
  * generate_baseline
    * Removed unnecessary try blocks (https://github.com/usnistgov/macos_security/issues/401[#401])
    * Update with correct syntax for replace (https://github.com/usnistgov/macos_security/pull/406[#406])
    * Support `.yaml` & .`yml` (https://github.com/usnistgov/macos_security/issues/412[#412])
  * generate_scap
    * Spelling fixes (https://github.com/usnistgov/macos_security/pull/409[#409])

## [Ventura, Revision 4.0] - 2024-04-24

* Rules
  * Modified Rules
    * os_anti_virus_installed (https://github.com/usnistgov/macos_security/issues/345[#345])
    * os_camera_disable (https://github.com/usnistgov/macos_security/issues/388[#388])
    * os_install_log_retention_configure (https://github.com/usnistgov/macos_security/issues/292[#292])
    * os_password_hint_remove (https://github.com/usnistgov/macos_security/issues/343[#343])
    * os_time_server_enabled (https://github.com/usnistgov/macos_security/issues/345[#345])
    * os_unlock_active_user_session_disable (https://github.com/usnistgov/macos_security/pull/365[#365])
    * system_settings_apple_watch_unlock_disable.yaml (https://github.com/usnistgov/macos_security/issues/326[#326])
    * system_settings_loginwindow_loginwindowtext_enable
    * system_settings_systemwide_preferences_configure
    * system_settings_time_server_configure.yaml (https://github.com/usnistgov/macos_security/pull/336[#336])
    * system_settings_touchid_unlock_disable.yaml (https://github.com/usnistgov/macos_security/issues/326[#326])
  * Other
    * Added tags to all supplemental rule files

* Scripts
  * generate_guidance
    * Added `--quiet` (https://github.com/usnistgov/macos_security/issues/301[#301])
    * Modified Configuration Profile Payload (https://github.com/usnistgov/macos_security/issues/315[#315])
    * Added `--audit` to compliance script (https://github.com/usnistgov/macos_security/pull/333/files[#333])
    * Added `--no-rcs`to zsh sheband (https://github.com/usnistgov/macos_security/issues/377[#377])
    * Bug Fixes
      * https://github.com/usnistgov/macos_security/issues/319[#319]
      * https://github.com/usnistgov/macos_security/issues/332[#332]
    * generate_baseline
      * Add tags to baselines (https://github.com/usnistgov/macos_security/issues/324[#324])
      * Bug Fixes
    * generate_mappings
      * Bug Fixes
    * generate_scap
      * Bug Fixes
  * Other
      * Added `util` folder
      * Added `generate_checklist.py`
      * Added `mscp_local_report.py`
      * Updated `enablePF-mscp.sh`

## [Ventura, Revision 3.0] - 2023-09-21

* Rules
  * Modified Rules
    * os_world_writable_system_folder_configure
    * os_hibernate_mode_apple_silicon_enable
    * os_hibernate_mode_destroyfvkeyonstandby_enable
    * os_hibernate_mode_intel_enable
    * os_ssh_fips_compliant
    * os_sshd_fips_compliant
    * system_settings_location_services_menu_enforce
    * system_settings_ssh_disable
  * Removed Rules
    * os_sshd_fips_140_ciphers
    * os_sshd_fips_140_macs
    * os_sshd_key_exchange_algorithm_configure

* Baselines
  * Modified
    * DISA-STIG
    * CISv8
    * cmmc_lvl2
    * cnssi-1253_low
    * cnssi-1253_moderate
    * cnssi-1253_high
    * all_rules

* Scripts
  * generate_guidance
    * Added iOS support
    * Added support for pwpolicy regex
    * Modified ssh_key_check
    * Bug Fixes
  * generate_baseline
    * Added iOS support
    * Bug Fixes
  * generate_mappings
    * Added iOS support
    * Bug Fixes
  * generate_scap
    * Added iOS support
    * Added support for pwpolicy regex
    * Bug Fixes

== [Ventura, Revision 2.0] - 2023-06-26

* Rules
  * Added Rules
    * os_home_folders_default
    * supplemental_stig
  * Modified Rules
    * audit_acls_files_configure
    * audit_acls_folders_configure
    * audit_auditd_enabled
    * audit_control_mode_configure
    * audit_files_group_configure
    * audit_files_mode_configure
    * audit_files_owner_configure
    * audit_folder_group_configure
    * audit_folder_group_configure
    * audit_folders_mode_configure
    * auth_ssh_password_authentication_disable
    * icloud_appleid_preference_pane_disable
    * icloud_appleid_system_settings_disable
    * os_anti_virus_installed
    * os_home_folders_secure
    * os_policy_banner_loginwindow_enforce
    * os_policy_banner_ssh_configure
    * os_policy_banner_ssh_enforce
    * os_screensaver_timeout_loginwindow_enforce
    * os_sshd_client_alive_count_max_configure
    * os_sshd_client_alive_interval_configure
    * os_sshd_fips_140_ciphers
    * os_sshd_fips_140_macs
    * os_sshd_fips_compliant
    * os_sshd_key_exchange_algorithm_configure
    * os_sshd_login_grace_time_configure
    * os_sshd_permit_root_login_configure
    * pwpolicy_account_lockout_timeout_enforce
    * pwpolicy_minimum_length_enforce
    * pwpolicy_special_character_enforce
    * system_settings_assistant_disable
    * system_settings_bluetooth_prefpane_disable
    * system_settings_firewall_enable
    * system_settings_firewall_stealth_mode_enable
    * system_settings_guest_account_disable
    * system_settings_internet_accounts_preference_pane_disable
    * system_settings_siri_prefpane_disable
    * system_settings_touch_id_pane_disable
    * system_settings_usb_restricted_mode
    * system_settings_wallet_applepay_prefpane_disable
    * system_settings_wallet_applepay_prefpane_hide

* Baselines
  * Added Baselines
    * cmmc_lvl1
    * cmmc_lvl2
    * cnssi-1253_high
    * cnssi-1253_moderate
    * cnssi-1253_low
    * DISA-STIG
  * Modified Baselines
    * all_rules
    * Removed Baselines
  * cnssi-1253

* Scripts
  * generate_guidance
    * Added base64 support for documentation logo
    * Added support for CMMC references
    * Added ssh key generation to compliance script
    * Added cfc argument to compliance script
    * Bug Fixes
  * generate_baseline
    * Bug Fixes
  * generate_scap
    * Bug Fixes

* Includes
  * mscp-data
    * Added CMMC data
    * Updated CNSSI-1253 data
  * supported_payloads
    * Added com.apple.sharingd
    * Removed com.apple.locationmenu

== [Ventura, Revision 1.1] - 2022-12-08

* Rules
  * Added Rules
    * icloud_game_center_disable
    * os_safari_advertising_privacy_protection_enable
    * os_safari_prevent_cross-site_tracking_enable
    * os_safari_show_full_website_address_enable
    * os_safari_warn_fraudulent_website_enable
  * Modified Rules
    * os_dvdram_disable
    * os_hibernate_mode_enable
    * os_rapid_security_response_removal_disable
    * os_tftpd_disable
    * system_settings_automatic_logout_enforce
    * system_settings_internet_accounts_disable
    * system_settings_ssh_enable
    * system_settings_system_wide_preferences_configure
    * system_settings_time_server_configure
    * system_settings_time_server_enforce
    * supplemental_cis_manual
  * Bug fixes

* Baselines
  * Updated all baselines

* Scripts
  * generate_guidance
    * Added custom references to compliance check script
    * Added debug option
    * Bug Fixes
  * generate_baseline
    * Added author function
    * Bug Fixes
  * generate_mapping
    * Bug Fixes

== [Ventura, Revision 1] - 2022-10-20

* Rules
  * Added ODV support
  * Added Rules
    * icloud_appleid_system_settings_disable
    * os_config_profile_ui_install_disable
    * os_firewall_ui_disable
    * os_power_nap_enable
    * os_rapid_security_response_allow
    * os_rapid_security_response_removal_disable
    * os_software_update_deferral
    * system_settings_USB_restricted_mode
    * system_settings_internet_accounts_disable
  * Modified Rules
    * os_power_nap_disable
    * os_ssh_fips_compliant
    * os_ssh_server_alive_count_max_configure
    * os_ssh_server_alive_interval_configure
    * os_sshd_client_alive_count_max_configure
    * os_sshd_client_alive_interval_configure
    * os_sshd_fips_140_ciphers
    * os_sshd_fips_140_macs
    * os_sshd_fips_compliant
    * os_sshd_key_exchange_algorithm_configure
    * os_sshd_login_grace_time_configure
    * os_sshd_permit_root_login_configure
    * os_sudo_timeout_configure
    * os_sudoers_timestamp_type_configure
    * pwpolicy_account_inactivity_enforce.yaml
    * pwpolicy_account_lockout_enforce.yaml
    * pwpolicy_account_lockout_timeout_enforce.yaml
    * pwpolicy_alpha_numeric_enforce.yaml
    * pwpolicy_history_enforce.yaml
    * pwpolicy_lower_case_character_enforce.yaml
    * pwpolicy_max_lifetime_enforce.yaml
    * pwpolicy_minimum_length_enforce.yaml
    * pwpolicy_minimum_lifetime_enforce.yaml
    * pwpolicy_simple_sequence_disable.yaml
    * pwpolicy_special_character_enforce.yaml
    * pwpolicy_upper_case_character_enforce.yaml
    * system_settings_system_wide_preferences_configure
    * System Preferences -> System Settings
  * Removed Rules
    * os_sudoers_tty_configure
  * Bug Fixes

* Baselines
  * Modified existing baselines
  * Added parent_values

* Scripts
  * generate_guidance
    * Added ODV support
    * Added Ruby gem generation
    * Added support for fix/check in compliance script
    * Added unified log support to compliance script
    * Bug Fixes
  * generate_baseline
    * Added ODV support
    * Added tailoring support
    * Bug Fixes
  * generate_mappings
    * Bug Fixes
  * generate_scap
    * Added support for ODV
    * Added support for new checks
    * Generate scap, xccdf, or oval
    * Bug Fixes
