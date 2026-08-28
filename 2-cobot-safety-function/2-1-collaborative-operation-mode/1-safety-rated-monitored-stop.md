# 2.1.1 Safety-rated monitored stop

The robot stops operating when a person enters the workspace. Either install an external monitoring device and connect it to the Safety Control Module (SCM) or use the radar sensor installed on the robot.

* When an external device is connected to the safety input, the stop modes (Stop0, Stop1, and Stop2) should be set in the safety input/output (I/O) signal setting.
* When a safeguard and an external emergency stop device are connected, the stop modes must meet the requirements of the international or local regulations.

The reference information on the setting of the related functions is as follows:

* For detailed information on radar module settings, please refer to ([8.1 Configuration procedure](https://hrbook-hrc.web.app/#/view/doc-Object-Detection-System/en/8-Configuration_and_Operation/8-1-Configuration_procedure/README?cont_model=${cont_model)) in the ([Function Manual - Radar Object DetectionSystem](https://hrbook-hrc.web.app/#/view/doc-Object-Detection-System/en/README?cont_model=${cont_model})).
* For detailed information on safety I/O signal settings, please refer to ([3.3.4 Safety Input/Output](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/en/3-safety-function/3-safety-function/4-safety-io/README?cont_model=Hi7%3Fcont_model%3D%24%7Bcont_model%7D?cont_model=${cont_model})) in the ([Hi7 Controller Function Manual - SafeSpace2.0](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/en/README?cont_model=%24%7Bcont_model%7D?cont_model=${cont_model})).
* For details on configuring the safe stop function, please refer to ([3.3.1.2 Stop Settings](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/en/3-safety-function/3-safety-function/1-general-condition/2-safe-stop?cont_model=Hi7?cont_model=${cont_model})) in the ([Hi7 Controller Function Manual - SafeSpace2.0](https://hrbook-hrc.web.app/#/view/doc-safespace2.0/en/README?cont_model=%24%7Bcont_model%7D?cont_model=${cont_model})).
