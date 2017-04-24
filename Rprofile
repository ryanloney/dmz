# colorout isn't on CRAN so install from source (it's easy)
# % git clone https://github.com/jalvesaq/colorout.git
# % R CMD INSTALL colorout

.First <- function()
{
	if (is.element('colorout', utils::installed.packages()[,1]) == T)
	{
		# Sys.getenv("TERM") %in% c("xterm-256color", "screen-256color"))
		library(colorout)
		setOutputColors256(string = 0, verbose = F)     # for solarized light
	}
}

# Set output width to size of the screen (if possible)
.set.width.option <- function()
{
	width = as.integer(Sys.getenv('COLUMNS'))
  if (!is.na(width))
  {
    options(width = width)
  }
}
.set.width.option()

