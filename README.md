# OGS Active Game Rank Updater

This script monitors the active games of a specific player on OGS (Online Go Server) and updates a configuration file based on the opponent's rank. 

## Prerequisites

- Python 3.x
- `requests` library (can be installed using `pip install requests`)

## Configuration

1. **Set Player ID:**
   - Replace `player_id` in the `main()` function with the OGS player ID you want to monitor.

2. **Set Configuration File Path:**
   - Update the `config_file_path` variable in the `main()` function with the path to the configuration file you want to modify.

## How It Works

1. **Fetch Active Games:**
   - The script queries the OGS API to get the active games for the specified player.

2. **Extract Opponent Information:**
   - For each active game, it determines the opponent and retrieves their rating.

3. **Update Configuration File:**
   - The script updates a specific line in the configuration file to reflect the opponent's rank based on their rating.

4. **Continuous Monitoring:**
   - The script continuously checks for active games every 2 seconds and updates the configuration file accordingly.

## Usage

1. **Run the Script:**
   - Execute the script using Python:

     ```sh
     python path/to/your_script.py
     ```

2. **Script Output:**
   - The script prints the updated rank label and the opponent's name to the console.

## Error Handling

- If the script encounters any issues (e.g., network errors or file read/write issues), it will print an error message to the console.

## License

This script is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact

For questions or feedback, please reach out to changcheng6541@gmail.com.

