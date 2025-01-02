# Insurance-Premium-ML


## Data
| Column Name                       | Description                                                                                  |
|-----------------------------------|----------------------------------------------------------------------------------------------|
| policy_id                         | The unique identifier for each insurance policy.                                             |
| policy_tenure                     | The length of time (in years) that the policy has been active.                               |
| age_of_car                        | The age of the insured car (in years) at the time the policy was taken.                      |
| age_of_policyholder               | The age of the policyholder (in years) at the time the policy was taken.                     |
| area_cluster                      | A categorical variable representing the cluster or category of the policyholder's residence. |
| population_density                | A measure of the population density in the policyholder's area of residence.                |
| make                              | The make or manufacturer of the insured car.                                                |
| segment                           | The segment or category of the insured car (e.g., compact, sedan, SUV).                     |
| model                             | The specific model or variant of the insured car.                                            |
| fuel_type                         | The type of fuel used by the insured car (e.g., petrol, diesel, electric).                  |
| max_torque                        | The maximum torque output of the car's engine.                                              |
| max_power                         | The maximum power output of the car's engine.                                               |
| engine_type                       | The type of engine used in the insured car (e.g., inline, V-type).                          |
| airbags                           | The number of airbags installed in the car.                                                 |
| is_esc                            | Binary: Does the car have electronic stability control (ESC)?                               |
| is_adjustable_steering            | Binary: Does the car have adjustable steering?                                              |
| is_tpms                           | Binary: Does the car have a tire pressure monitoring system (TPMS)?                         |
| is_parking_sensors                | Binary: Does the car have parking sensors?                                                  |
| is_parking_camera                 | Binary: Does the car have a parking camera?                                                 |
| rear_brakes_type                  | The type of rear brakes used in the car.                                                    |
| displacement                      | The engine displacement (typically measured in liters or cubic centimeters).                |
| cylinder                          | The number of cylinders in the car's engine.                                                |
| transmission_type                 | The type of transmission used in the car (e.g., manual, automatic).                         |
| gear_box                          | The number of gears in the car's gearbox.                                                   |
| steering_type                     | The type of steering system used in the car.                                                |
| turning_radius                    | The minimum radius of the circular path the car can make.                                   |
| length                            | The length of the car.                                                                       |
| width                             | The width of the car.                                                                        |
| height                            | The height of the car.                                                                       |
| gross_weight                      | The gross weight or total weight of the car.                                                |
| is_front_fog_lights               | Binary: Does the car have front fog lights?                                                 |
| is_rear_window_wiper              | Binary: Does the car have a rear window wiper?                                              |
| is_rear_window_washer             | Binary: Does the car have a rear window washer?                                             |
| is_rear_window_defogger           | Binary: Does the car have a rear window defogger?                                           |
| is_brake_assist                   | Binary: Does the car have a brake assist system?                                            |
| is_power_door_locks               | Binary: Does the car have power door locks?                                                 |
| is_central_locking                | Binary: Does the car have central locking?                                                  |
| is_power_steering                 | Binary: Does the car have power steering?                                                   |
| is_driver_seat_height_adjustable  | Binary: Is the driver's seat height adjustable?                                             |
| is_day_night_rear_view_mirror     | Binary: Does the car have a day/night rearview mirror?                                       |
| is_ecw                            | Binary: Does the car have an electronic crash warning (ECW) system?                         |
| is_speed_alert                    | Binary: Does the car have a speed alert system?                                             |
| ncap_rating                       | The safety rating of the car based on NCAP (star rating).                                   |
| is_claim (Target Variable)        | Binary: Was an insurance claim filed? (1 = Yes, 0 = No)                                     |
