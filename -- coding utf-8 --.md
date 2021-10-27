# -*- coding: utf-8 -*-
"""
Created on Sat Oct  9 10:20:21 2021

@author: eirik
"""

class Multiple_choice:
    
    def __init__(self,question,answer_1,answer_2,answer_3,correct_answer):
        self.question = question
        self.answer_1 = answer_1
        self.answer_2 = answer_2
        self.answer_3 = answer_3
        self.correct_answer = correct_answer
        
    def set_answer_1(self,new_answer_1):
        self.answer_1 = new_answer_1
    
    def set_answer_2(self,new_answer_2):
        self.answer_2 = new_answer_2
        
    def set_answer_3(self,new_answer_3):
        self.answer_3 = new_answer_3
        
    def set_correct_answer(self,new_correct_answer):
        self.correct_answer = new_correct_answer
    
    def get_answer_1(self):
        return self.get_answer_1
    
    def get_answer_2(self):
        return self.get_answer_2
        
    def get_answer_3(self):
        return self.get_answer_3
        
    def get_correct_answer(self):
        return self.get_correct_answer
    
    def __str__(self):
        print(self.question)
        print('Choice 1 is: ' + str(self.answer_1))
        print('Choice 2 is: ' + str(self.answer_2))
        print('Choice 3 is: ' + str(self.answer_3))
        
    def answer_check(self,guess):
        if self.correct_answer == guess:
            print('Correct!')
        else:
            print('No, that is not the correct answer')


​        
#Question 1
question_component =  'What year did Christoffer Columbus first arrive in America?'
answer_component_1 = '1492'
answer_component_2 = '1501'
answer_component_3 = '1470'
correct_answer_component = str(1)


question_1 = Multiple_choice(question_component,answer_component_1,answer_component_2,answer_component_3,correct_answer_component)

question_1.__str__()

guess = input('Guess the correct question (1/2/3): ')

question_1.answer_check(guess)

#Question 2
question_component =  'Who is considered the inventor of capitalism?'
answer_component_1 = 'Karl Marx'
answer_component_2 = 'Friedrich Nietzche'
answer_component_3 = 'Adam Smith'
correct_answer_component = str(3)


question_2 = Multiple_choice(question_component,answer_component_1,answer_component_2,answer_component_3,correct_answer_component)

question_2.__str__()

guess = input('Guess the correct question (1/2/3): ')

question_2.answer_check(guess)