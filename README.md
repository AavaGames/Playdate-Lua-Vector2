# Playdate-Lua-Vector2
Made by Hasnain Raza

Additions by Philip Fertsman (@aavagames)
	
	Add-on to Hasnain's Vector2 lua class for the Playdate. 
	Additions: Clamp, Lerp, Convienance "Vector2.Zero()"

	Original Note: It is recommended that you rely on arithmetic operators rather than calling functions
	because error handling is done primarily on the operators.

# Installation

Just drop in your project and import.

## Example
	local position = Vector2.zero() same as Vector.new(0, 0)
	
	self.moveDir = Vector2.zero()
	if playdate.buttonJustPressed(playdate.kButtonRight) then
            self.moveDir.x += 1
        end
	
	position += moveDir
	self:moveTo(position)
