src=$(wildcard ./*.cpp)
object=$(patsubst %.cpp,%.o,$(src))
target=main
$(target):$(object)
	g++ -o $@ $^
%.o:%.cpp
	g++ -o $@ -c $< $(CPPFLAGS)
.PHONY:clean
clean:
	-rm -f $(target) $(object)