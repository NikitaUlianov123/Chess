# Chess

A multiplayer chess game in C# (2022), with a MonoGame client and an ASP.NET Core server.

## What's here

- **SharedLibrary**: the game rules: pieces, moves, and pawn promotion. It includes a **Crazyhouse** variant, where captured pieces can be dropped back onto the board.
- **WebApi2**: the game server. `ChessController` creates games, assigns players and colors, returns legal moves, and applies moves.
- **Chess**: the MonoGame client, with a menu and screens for normal and Crazyhouse games. Players join a game with a shared game ID.

The client reads the server address from the `ServerBaseURL` app setting.
